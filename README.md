# Task Planning Agent using Chain-of-Thought, Tree-of-Thought and ReAct

## 📌 Project Overview

This project demonstrates an AI-style task-planning system that uses structured reasoning, goal decomposition, Tree-of-Thought (ToT), and the ReAct (Reason + Act) framework to solve a multi-step planning problem.

The system is developed using Python and demonstrates how an agent can break a complex goal into smaller tasks, evaluate different possible solutions, interact with tools, observe changes in the environment, and replan when its original assumptions become incorrect.

**Shared Task:** Plan a one-day trip within a budget of ₹600, starting at 8:00 AM and returning before 9:00 PM, while ensuring a minimum stay of four hours at the selected destination.

## 🎯 Objectives

- Break a complex goal into smaller, ordered subtasks.
- Understand how Chain-of-Thought-style structured reasoning supports planning.
- Use Tree-of-Thought to evaluate multiple possible plans.
- Implement a ReAct-style reasoning and tool-use loop.
- Observe environmental changes using tools.
- Trigger replanning when an assumption is violated.
- Understand how an agent handles situations where no valid plan is available.

## 🧠 Concepts Implemented

### 1. Chain-of-Thought (CoT) – Structured Reasoning

The system breaks the main travel goal into smaller steps and explains why each step is required.

The subtasks include:
1. Choose a destination and transport option.
2. Check weather conditions.
3. Check transport availability.
4. Book transport.
5. Perform a final weather check.
6. Generate the final itinerary.

A dependency graph ensures that tasks are performed in the correct order.

### 2. Tree-of-Thought (ToT) – Exploring Multiple Options

Instead of selecting the first available destination, the system evaluates multiple
