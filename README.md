
# Project Scheduling System

The Project Scheduling System is a C++ program designed to facilitate project management. It offers features such as adding resources, defining tasks, calculating project schedules, and managing resource allocation based on availability and proficiency.

# Table of contents (TOC)

- Features
- Prerequisites
- How to Use
- Code Explanation
- References


## Features

- **Resource Management:** Add and manage project resources, including details like skill, proficiency, and availability.
- **Task Definition:** Define project tasks with parameters such as duration, skill requirements, and dependencies.
- **Schedule Calculation:** Utilize the Critical Path Method (CPM) to calculate the project's basic schedule.
- **Resource Availability:** Calculate project completion time while considering resource availability.
- **Resource Proficiency:** Calculate project completion time while considering resource proficiency.
- **Schedule Visualization:** Print the project schedule for easy reference.
- **User-Friendly Interface:** Navigate the system using a user-friendly menu-driven interface.

## Prerequisites

- **C++ Compiler:** Ensure you have a C++ compiler installed (C++11 or later).
- **Basic C++ Knowledge:** Familiarity with C++ programming is recommended.

## How to Use

1. **Clone or Download:** Obtain the source code by cloning this repository or downloading it to your local machine.

2. **Compile:** Compile the source code using a C++ compiler with the following command:

    ```bash
    g++ -o project_scheduler main.cpp
    ```

3. **Run:** Execute the compiled program:

    ```bash
    ./project_scheduler
    ```

4. **Interact:** Use the menu-driven interface to interact with the Project Scheduling System. Add resources, define tasks, calculate schedules, and more.

## Code Explanation

The code is structured around several classes, including Skill, Resource, Task, and Project. Here's a brief overview:

- **Skill:** Represents a skill with an ID, name, and proficiency level.
- **Resource:** Represents a resource with an ID, name, associated skill, availability, and start time.
- **Task:** Represents a task with an ID, name, duration, associated skill, dependencies, start time, early start time, slack, and successors.
- **Project:** Represents the project itself, containing resources and tasks.

Key functions in the program include:

- `addResources`: Allows users to input resource details and adds them to the project.
- `addTasks`: Allows users to input task details, including dependencies, and adds them to the project.
- `calculateBasicSchedule`: Calculates the basic project schedule using CPM.
- `completionTimeWithResources`: Calculates project completion time considering resource availability.
- `completionTimeWithResourceProficiency`: Calculates project completion time considering resource proficiency.
- `printSchedule`: Displays the project schedule.

## References

This project's code is a basic implementation of a project scheduling system. It does not rely on specific external references or libraries but is based on the principles of the Critical Path Method (CPM) for project scheduling.

For additional information on C++, you can refer to the [C++ documentation](https://www.cplusplus.com/).

