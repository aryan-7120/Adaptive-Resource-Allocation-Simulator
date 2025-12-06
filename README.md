# Adaptive-Resource-Allocation-Simulator
Adaptive Resource Allocation Simulator in Multiprogramming Systems

This project is a Python-based simulator designed to visualize how modern operating systems manage CPU and memory allocation in a multiprogramming environment. It demonstrates real-time scheduling, adaptive resource distribution, and process state transitions using an interactive Tkinter GUI.

⭐ Project Overview

Modern operating systems run multiple processes concurrently, and efficiently allocating resources like CPU and memory is essential for performance and stability.
This simulator provides a visual and interactive way to observe:

How processes request and consume resources

How states like Ready, Running, Waiting, and Completed change

How a scheduler distributes CPU time

How memory limits affect executions

🧩 System Architecture (Three Modules)
1️⃣ Module 1 — Process Management

Handles:

Creating new processes

Assigning unique PIDs

Tracking CPU & memory requests

Managing process states

Deleting processes

Resetting the simulation

This module forms the backbone of the entire simulator.

2️⃣ Module 2 — Resource Allocation & Scheduling

Responsible for:

Checking memory availability

Dynamically distributing CPU among running processes

Moving processes between Ready → Running → Waiting → Completed

Updating progress in real-time

This module makes the system adaptive and ensures no over-allocation happens.

3️⃣ Module 3 — Graphical User Interface (GUI)

Built using Tkinter, the GUI includes:

CPU usage bar (0–100%)

Memory usage bar (0–2048 MB)

Table showing all processes

Progress bars for each running process

Add / Delete / Reset buttons

Sliders for CPU & memory before adding a process

Real-time updates

This module makes the simulator easy and intuitive to understand.

⚙️ How the Simulator Works
Process States

Ready → Waiting for CPU/Memory to start execution

Running → Actively executing, consuming resources

Waiting → Paused due to insufficient resources

Completed → Finished and resources freed

Adaptive Scheduling Algorithm

A process starts running only if enough memory is available

CPU is fairly split among running processes

Progress updates live until the process completes

Completed processes release CPU & memory back to the system

🛠️ Tech Stack: 

Python

Tkinter (GUI)

Threading (background scheduling loop without freezing GUI)

psutil (system information)

Time (interval-based updates)

Treeview & Progressbars (visual feedback)

▶️ How to Run the Project
1. Install dependencies
pip install psutil


Tkinter comes pre-installed with Python.

2. Run the simulator
python main.py

📸 Features Demonstrated

Real-time CPU & memory usage visualization

Dynamic creation & deletion of processes

Adaptive scheduling

Progress indicators for all processes

Memory-bound execution control

Clean and simple GUI

💡 Key Learnings

CPU scheduling concepts

Memory management

Multiprogramming simulation

GUI development using Tkinter

Threading for concurrency
