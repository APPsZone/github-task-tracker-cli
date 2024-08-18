# Task Tracker CLI (Command Line Interface)

Task Tracker CLI is a feature that allows us to add, update, mark, and also delete task in JSON file with a simple command line application in it. It also let us view a list of task based on their status.

## Features
- **Add**: Add a new task with a description and a default status of "todo",
- **List**: View tasks based on their status (todo, in progress, done, or all).
- **Update**: Update the description of an existing task based on their ID.
- **Mark**: Change the status of a task into "in progress" or "done" based on their ID.
- **Delete**: Remove an existing task based on their ID.

## Usage

### Add Task

To add a new task, use the `-a` or `--add` argument:

```bash
pytho tracker.py -a "Add a New Task"
```

### List Tasks

To list tasks based on their status, use the `-l` or `--list` argument. You can specify it into "todo", "in progress", "done", or "all":

```bash
python tracker.py -l "todo"
```

### Update Task Description

To update the description of a task, use the `-p` (pick) argument to specify the task ID and the `-u` (update) argument to provide the new description:

```bash
python tracker.py -p 2 -u "Updated Task Description"
```

### Mark Task Status

To mark a task as "in progress" or "done", use the `-p` (pick) argument to specify the task ID and the `-m` (mark) argument to provide the new status:

```bash
python tracker.py -p 2 -m "in progress"
```

### Delete Task

To delete a task, use the `-p` (pick) argument to specify the task ID and the `-d` (delete) argument:

```bash
python tracker.py -p 2 -d "del"
```

## Notes

- Ensure that the `task_tracker.json` file exists in the same directory as the script for it to function correctly.
- The application will create the `task_tracker.json` file if it does not already exist when adding a new task.

## Project Link

For further information about this project, visit the [Task Tracker Project Roadmap](https://roadmap.sh/projects/task-tracker).# github-task-tracker-cli
