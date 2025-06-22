# productivity_app

# Productivity Timer

A simple, terminal-based productivity app to help you stay focused and manage your work sessions based on a predefined schedule.

## Description

This script helps you follow a structured schedule by timing your tasks. It loads a list of tasks and their durations from a `tasks.json` file, and then displays a running timer for each task. It's a great tool to enforce discipline for routines like studying, working on projects, or following a trading plan.

The idea is inspired by the "RBI" process for algorithmic trading:
- **R**esearch strategies.
- **B**acktest them to validate.
- **I**mplement the profitable ones.

## Features

- **Task scheduling**: Loads tasks and durations from an external `tasks.json` file.
- **Live Timer**: Displays the current task with remaining time.
- **Visual Alerts**: The color of the current task changes to red when time is running out, providing a clear visual cue.
- **Motivational Quotes**: Shows a random motivational quote to keep you going.
- **Completion message**: Notifies you when all tasks for the session are completed.

## Requirements

- Python 3
- `termcolor`

You can install the necessary package using pip:
```bash
pip install termcolor
```

## Usage

1.  **Configure your tasks**:
    Open the `tasks.json` file and modify it to define your own list of tasks and their duration in minutes.
    ```json
    {
        "Task 1": 30,
        "Task 2": 60,
        "Task 3": 15
    }
    ```

2.  **Run the application**:
    Navigate to the application directory and run the script from your terminal:
    ```bash
    python productivity.py
    ```

## Customization

### Tasks
You can customize the tasks and their durations by editing the `tasks.json` file. The key is the task name (a string), and the value is the duration in minutes (an integer).

### Reminders
You can change the list of motivational reminders by editing the `list_of_reminders` variable inside the `productivity.py` script.

```python
# ... inside productivity.py
        list_of_reminders = [
            "Your new reminder here",
            "Another great quote",
        ]
# ...
``` 
