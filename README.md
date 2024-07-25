# Coding_Challenge1-
Introduction:

We're going to build a task scheduler that calculates the earliest and latest completion times for a series of tasks with dependencies.
Class Initialization:

__init__: Initializes the task scheduler with dictionaries to store task durations, dependencies, and finish times (EFT and LFT).
Add Task:

add_task(task_id, duration): Adds a task with its duration.
Add Dependency:

add_dependency(from_task, to_task): Adds a dependency between tasks.
Calculate Times:

calculate_times(): Calculates both earliest and latest finish times.
Calculate Earliest Times:

calculate_earliest_times(): Uses topological sorting to determine the earliest finish times for each task. It starts with tasks having no dependencies, and then iterates through the dependencies updating EFT.
Calculate Latest Times:

calculate_latest_times(): Propagates the latest finish times from the end tasks backward using a similar approach but with reversed dependencies.
Completion Times:

earliest_completion_time(): Returns the earliest time by taking the max of EFT.
latest_completion_time(): Returns the latest time by taking the max of LFT.
Example Usage:

Demonstrates how to use the TaskScheduler class to add tasks, dependencies, and calculate the completion times.
