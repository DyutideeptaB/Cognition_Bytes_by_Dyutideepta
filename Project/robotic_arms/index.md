---
layout: page
title: ""
permalink: /Project/robotic_arms/
---

# 🤖 Dual-Arm Robotic System Synchronisation

## Visual-Guided Decentralised Coordination in PyBullet

------------------------------------------------------------------------

### 📌 Overview

This project implements a **dual-arm robotic system** in simulation, where:

-   A **UR3 manipulator (Worker)** performs object manipulation and trajectory execution
-   A **Franka Emika Panda (Observer)** provides visual feedback via an eye-in-hand camera

The system demonstrates **decentralised coordination**, where:

> No direct joint/state sharing exists between robots --- coordination
> emerges purely through **vision-based feedback and control loops**.

The primary task involves: - Picking a cube using visual estimation
- Executing a smooth **infinity (∞) trajectory**
- Maintaining continuous visual tracking under noise and occlusion

------------------------------------------------------------------------

### 🧠 Core Contributions

-   🔄 **Decentralised dual-arm coordination**
-   👁️ **Visual servoing using image-space error**
-   📐 **Mathematical trajectory modelling (Lissajous curve)**
-   ⚙️ **Physics-based simulation (PyBullet)**
-   📊 **Logging + performance evaluation pipeline**
-   🧩 **Robust state-machine-driven control (both robots)**

------------------------------------------------------------------------

### 🏗️ System Architecture

            Camera (Franka - Eye-in-Hand)
                        │
            RGB Frame → HSV Detection → Centroid (cx, cy)
                        │
                Pixel Error (ex, ey)
                        │
             v_cam → v_world (via R_cam)
                        │
         Jacobian-based Control (DLS Inverse)
                        │
             Franka Joint Velocity Update
                        │
            ─────────────────────────────
                        │
            Stable 3D Estimate (Y, Z)
                        │
                  UR3 State Machine
                        │
        Pick → Lift → Infinity Trajectory

------------------------------------------------------------------------

### ⚙️ Mathematical Foundations

#### 📌 Infinity Trajectory (Lissajous Curve)

    y(t) = C_Y + A_Y sin(ωt)
    z(t) = C_Z + A_Z sin(2ωt)

------------------------------------------------------------------------

#### 📌 Visual Servoing Control

Pixel error:

    e_x = c_x - W/2
    e_y = c_y - H/2

Camera velocity:

    v_cam = [ 0,
              K_pix * e_x,
             -K_pix * e_y ]

Jacobian-based control:

    q_dot = J^T (J J^T + λI)^(-1) v_world

------------------------------------------------------------------------

### 🔄 Control Logic

#### 🦾 UR3 (Worker Arm)

Finite state machine:

1.  **WAIT_FOR_CAM** -- waits for stable visual estimate
2.  **APPROACH** -- moves to pick position
3.  **LIFT** -- lifts object to safe pose
4.  **MOVE\_∞** -- executes infinity trajectory

Smoothing:

    p_smooth = α p_ref + (1 - α) p_smooth

------------------------------------------------------------------------

#### 👁️ Franka (Observer Arm)

#### Detection Pipeline

-   RGB → HSV conversion
-   Red colour thresholding
-   Centroid detection

##### Tracking States

-   SEARCH
-   TRACKING
-   TEMP_LOST
-   LOST

##### Control

-   Pixel error → velocity
-   Jacobian inverse
-   Velocity clipping

------------------------------------------------------------------------

### 📦 Movement_with_logs.py (Enhanced Implementation)

#### 📊 Logging System

-   Pixel error: `e_x(t), e_y(t)`
-   End-effector error: `e_EE(t) = || p_EE(t) - p_ref(t) ||`

------------------------------------------------------------------------

#### 🔁 Stability Improvements

-   First-order smoothing
-   Buffered cube position estimation
-   Cluster-based validation

------------------------------------------------------------------------

#### 🧩 Robustness Features

-   Handles noisy detections
-   Handles occlusions
-   Multi-frame consistency checks
-   Kalman Filter for pose estimation

------------------------------------------------------------------------

### 🚀 Tech Stack

-   Python
-   PyBullet
-   NumPy
-   OpenCV

------------------------------------------------------------------------

### ▶️ How to Run

``` bash
git clone https://github.com/DyutideeptaB/Dual-Arm_Robotic_System_Synchronisation.git
cd Dual-Arm_Robotic_System_Synchronisation
pip install -r requirements.txt
python Final_with_logs.py
```

------------------------------------------------------------------------

### 📊 Outputs

-   Pixel error vs time
-   End-effector tracking error
-   Infinity trajectory (reference vs actual)

------------------------------------------------------------------------

### 🔬 Applications

-   Collaborative robotics
-   Industrial automation
-   Visual servoing research
-   Multi-agent systems

------------------------------------------------------------------------

### 📈 Future Work

-   Reinforcement learning integration
-   Real robot deployment
-   Multi-object tracking
-   Dynamic environments

------------------------------------------------------------------------

### 👤 Author

**Dyutideepta Banerjee**\
Physics + AI \| Simulation Driven Systems \| Computer Vision

------------------------------------------------------------------------

### ⭐ Final Note

This project demonstrates how **coordinated robotic behaviour can emerge
purely from perception-driven feedback**, without centralised control.

<div style="display: flex; justify-content: flex-start; align-items: center; max-width: 800px; margin: 10px auto; font-size: 0.95em;">
  <a href="https://github.com/DyutideeptaB/Dual-Arm_Robotic_System_Synchronisation" target="_blank" style="text-decoration: none; color: #007bff; display: flex; align-items: center;">
    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/github.svg" alt="GitHub" width="20" height="20" style="margin-right: 6px;">
    View GitHub Repository
  </a>
</div>

