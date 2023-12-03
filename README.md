# Task Management App

This simple task management application allows users to add, remove, list tasks, and receive task recommendations based on a machine learning model.

## Prerequisites
- Python 3.x
- pandas
- scikit-learn

## Setup
1. Make sure you have Python 3.x installed on your system.
2. Install the required dependencies using the following command:
    ```bash
    pip install pandas scikit-learn
    ```

## Usage
1. Run the script in a Python environment.
    ```bash
    python your_script_name.py
    ```
2. The main menu will be displayed with the following options:
   - **1. Add Task:** Add a new task to the list.
   - **2. Remove Task:** Remove a task based on its description.
   - **3. List Tasks:** Display all existing tasks.
   - **4. Recommend Task:** Get a random high-priority task recommendation.
   - **5. Exit:** Quit the application.

## Features
- The application stores tasks in a CSV file (`tasks.csv`) and loads them on startup.
- Task priority is determined using a simple Naive Bayes classifier trained on task descriptions.
- Users can interact with the application through a text-based menu.

## Functions
- **add_task(description, priority):** Adds a new task to the task list and saves it to the CSV file.
- **remove_task(description):** Removes a task based on its description and saves the updated task list.
- **list_tasks():** Displays all tasks currently in the list.
- **recommend_task():** Recommends a random high-priority task using the trained machine learning model.

## Machine Learning Model
The application utilizes a simple text classification model based on the Multinomial Naive Bayes algorithm. The model is trained on task descriptions to predict task priorities.

## Note
- Make sure to handle exceptions appropriately when interacting with the application, especially file-related operations.
- The CSV file (`tasks.csv`) is used for persistence, so avoid modifying it manually unless you understand the data format.

Feel free to customize and extend the functionality based on your needs!
