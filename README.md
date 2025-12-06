# Adaptive-Resource-Allocation-Simulator

Adaptive Resource Allocation Simulator in Multiprogramming Systems

This Python project is a simulator that visualizes how operating systems manage CPU and memory allocation in a multiprogramming environment. It demonstrates real-time scheduling, dynamic resource distribution, and process state transitions using an interactive Tkinter GUI.

⭐ Project Overview

Modern operating systems run multiple processes concurrently. Efficient allocation of resources like CPU and memory is crucial for performance and stability.
This simulator provides a visual and interactive way to observe:

How processes request and consume CPU and memory

How process states like Ready, Running, Waiting, and Completed change dynamically

How the scheduler distributes CPU time fairly

How memory constraints affect execution

🧩 System Architecture (Three Modules)
1️⃣ Module 1 — Process Management

Handles:

Creating new processes

Assigning unique Process IDs (PIDs)

Tracking CPU & memory requirements

Managing process states

Deleting processes

Resetting the simulator

This module forms the core of the simulator.

2️⃣ Module 2 — Resource Allocation & Scheduling

Responsible for:

Checking memory availability before running a process

Dynamically distributing CPU among running processes

Updating process states (Ready → Running → Waiting → Completed)

Updating progress bars in real-time

This module ensures adaptive allocation and prevents resource overuse.

3️⃣ Module 3 — Graphical User Interface (GUI)

Built with Tkinter, this module includes:

CPU usage bar (0–100%)

Memory usage bar (0–2048 MB)

Table listing all processes

Black progress bars for each process

Add / Delete / Reset buttons

Sliders to set CPU & memory before adding a process

Real-time updates

This module makes the simulator interactive and easy to understand.

⚙️ How the Simulator Works
Process States

Ready: Waiting for CPU or memory to start execution

Running: Actively executing and consuming resources

Waiting: Paused due to insufficient resources

Completed: Finished execution and resources released

Adaptive Scheduling Algorithm

A process only runs if enough memory is available

CPU is fairly split among all running processes

Progress updates live until process completion

Completed processes release CPU & memory back to the system

🛠️ Tech Stack

Python – main programming language

Tkinter – GUI toolkit

Threading – background scheduler without freezing UI

psutil – for system resource info

Time – for interval-based updates

Treeview & Progress Bars – for visualization

▶️ How to Run the Simulator

Install dependencies:

pip install psutil


Tkinter comes pre-installed with Python.

Run the simulator:

python main.py

📸 Features

Real-time CPU & memory visualization

Dynamic process creation and deletion

Adaptive scheduling based on resource availability

Progress bars for all processes

Memory-bound execution control

Clean, simple, and interactive GUI

💡 Key Learnings

CPU scheduling and allocation

Memory management strategies

Multiprogramming simulation

GUI development with Tkinter

Threading for concurrency and responsive interface