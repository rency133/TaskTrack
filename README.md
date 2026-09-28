# TaskTrack

TaskTrack is a command-line task manager created for CPS 310.

## Current Features

- Displays a menu for the user to choose from
- Adds user-entered tasks to a list, ignores blank input
- List is saved even after program is closed in a text file (tasks.txt)
- Gives the option for the user to display the list of tasks
    along with assigning each task a number

## Requirements
- Python 3

## Project Files

- `tasktrack.py` - The file that compiles and runs. Displays menu, takes user input, and saves tasks as a list.
- `tasks.txt` - Text file that holds all tasks.
- `.gitignore` - A list of files to ignore.

## Running the Program

Within project folder in Python: Hover over 'Terminal' in the top left corner. A sub-list will pop up with options, click on the one that says 'New Terminal'. Run the following command in Windows: 

```text
python tasktrack.py
```

## Task Persistence

Tasks are loaded at the beginning of the program. When a non-empty task is added using the add_task function, the task is saved and written to `tasks.txt`.

## Sample Interaction

```text
enter in terminal: 
python tasktrack.py

you will be prompted to choose from the menu choosing 1-3 until you enter '3':
1. View Tasks
2. Add Task
3. Exit

'1' will show you the current saved tasks for example:
Tasks:
1. Complete ICA04
2. Review GitHub commands

'2' will allow you to enter a task:
'Finish Assignment 1'

If you want to view all tasks after adding one, press '1' and you would get:
Tasks:
1. Complete ICA04
2. Review GitHub commands
3. Finish Assignment 1

'3' will exit the program, but your tasks will be saved in tasks.txt
GoodBye!
```

## Current Limitation

The program currently does not have a delete function. If you want to delete a task, you have to manually delete it from the `tasks.txt` file.