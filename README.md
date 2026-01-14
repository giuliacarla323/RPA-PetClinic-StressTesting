# Automated Stress Testing Robot (UiPath RPA)

This project features an advanced RPA solution developed in **UiPath** designed to perform automated stress testing on a Spring Framework application (Pet Clinic). The goal was to replace tedious manual testing with a robust, scalable, and parallel-executed robotic process.

## 🚀 Key Features

- **End-to-End Automation**: Automates the "Add Owner" and "Find Owner" functionalities.
- **Parallel Execution**: Implemented parallelization to simulate concurrent user interactions and measure system stability.
- **Data-Driven Approach**: Processes test data dynamically from external CSV files.
- **Fuzzy Selectors**: Utilizes resilient selectors to ensure the robot remains functional despite minor UI inconsistencies.
- **Automated Reporting**: Generates comprehensive test results in a structured table, including timestamps and success/fail status.

## 🏗️ Layered Architecture

The project follows a professional modular structure:
1. **TestCase**: Entry point for initializing test scenarios.
2. **Main**: Orchestrates the flow and manages global variables.
3. **Input**: Handles data retrieval from CSV sources.
4. **Parallel**: Manages concurrent execution threads.
5. **Process**: Executes the actual UI interactions and business logic.

## 🛠️ Tech Stack
- **Tool**: UiPath Studio
- **Language**: VB.NET (expressions within activities)
- **Data Formats**: CSV, DataTable
- **Target App**: Pet Clinic (Spring Framework)

## 📈 Challenges Overcome
- **Parallelization Complexity**: Managed data synchronization between parallel threads.
- **Fuzzy Matching**: Optimized selectors to reduce "SelectorNotFound" exceptions.
- **Error Handling**: Implemented a global `Try-Catch` strategy with detailed logging for debugging "site server failures."

## 🏁 Conclusion
Automated testing with UiPath significantly reduced human error and execution time compared to manual stress testing, providing valuable insights into server performance under high load.
