# energy_efficient.1
Overview
This project implements an Energy-Optimized Task Scheduler (EOTS) that dynamically adjusts CPU frequency levels to balance energy consumption and task deadlines. It uses Tkinter for the graphical interface and matplotlib for Gantt chart visualization.

Features
Implements Priority Scheduling, Earliest Deadline First (EDF), Round Robin, and Hybrid Energy-Aware Priority Scheduling.
Simulates multi-core CPU scheduling.
Adjusts CPU frequency dynamically based on task priority and slack time.
Tracks energy consumption per core.
Displays Gantt chart visualization.
Logs task execution details.

Dependencies
Ensure you have the following Python libraries installed:
pip install matplotlib tkinter

Usage
Run the script using:
python cpu_scheduling.py

Interface
Task Configuration: Allows defining task priorities, execution times, and deadlines.
Core Management: Displays core utilization and energy consumption.
Gantt Chart: Visualizes task execution across CPU cores.
Logs: Provides execution details per task.

CPU Frequency Levels
The system adjusts CPU frequency dynamically based on slack time:
Low (0.8 GHz, power: 0.5 units, green) - Used for tasks with high slack.
Mid (1.2 GHz, power: 1.0 units, yellow) - Balanced frequency for moderate slack.
High (2.0 GHz, power: 2.0 units, red) - Used for high-priority tasks or tight deadlines.

Scheduling Algorithms
Priority Scheduling - Tasks with higher priority execute first.
EDF (Earliest Deadline First) - Executes tasks closest to their deadline.
Round Robin - Time-slice based scheduling for fairness.
Hybrid Energy-Aware Priority Scheduling - Dynamically adjusts frequency for energy efficiency.

