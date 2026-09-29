# Capstone Proposal: Student Task and Deadline Manager

**Student:** Kevin Naindouba
**Course:** EGN 310: Data Structures (Fall A 2026)
**Language:** Python
**Project Type:** Command-Line Application

## 1. Problem

Students often manage assignments, quizzes, exams, and personal deadlines across multiple courses. When several deadlines overlap, it becomes difficult to determine which task requires attention first. This project will address that problem by creating a Student Task and Deadline Manager that organizes academic tasks and helps students identify their upcoming priorities.

## 2. Data Structure and Justification

The primary data structure will be a **priority queue implemented using a binary min-heap**. Each task will contain a title, course name, due date, and priority level. Tasks will be organized so that the most urgent task can be accessed first.

A priority queue is appropriate because the application needs to repeatedly identify and retrieve the next task requiring attention. Compared with an ordinary unsorted list, which requires scanning all tasks to find the earliest deadline, a binary heap provides O(1) access to the highest-priority task and O(log n) insertion and removal. This makes task management more efficient as the number of assignments increases.

A dictionary will also be used to store tasks by their unique IDs, allowing efficient lookup and updates.

## 3. Planned Features by Module 8

1. **Task Creation:** Add academic tasks with a title, course, due date, and priority level.

2. **Priority-Based Organization:** Automatically organize tasks using a priority queue so the most urgent task appears first.

3. **Task Management:** View, update, and remove tasks, including marking completed assignments.

4. **Deadline Dashboard:** Display pending tasks, completed tasks, and the next upcoming deadline, with clear warnings for overdue assignments.

## 4. Expected Outcome

By Module 8, the project will deliver a functional Python command-line application demonstrating practical use of a priority queue and dictionary. The application will help students organize academic responsibilities while demonstrating how appropriate data structures improve task retrieval and management.
