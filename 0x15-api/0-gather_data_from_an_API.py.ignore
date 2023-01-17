#!/usr/bin/python3
"""
Using https://jsonplaceholder.typicode.com
returns info about employee TODO progress

This script need some more thinking...for later

"""
import requests
from sys import argv


def request_data():
    """Requests employees data and TODO"""
    employees = requests.get("https://jsonplaceholder.typicode.com/users")
    EMPLOYEE_NAME = ""
    for employee in employees.json():
        if employee.get("id") == int(argv[1]):
            EMPLOYEE_NAME = employee.get("name")
            break
    NUMBER_OF_DONE_TASKS = 0
    TOTAL_NUMBER_OF_TASKS = 0
    TASK_TITLE = []

    tasks = requests.get("https://jsonplaceholder.typicode.com/todos")
    for task in tasks.json():
        if task.get("userId") == int(argv[1]):
            TOTAL_NUMBER_OF_TASKS += 1
            if task.get("completed") is True:
                NUMBER_OF_DONE_TASKS += 1
                TASK_TITLE.append(task.get("title"))

    print(
        f"Employee {EMPLOYEE_NAME} is done with"
        f" {NUMBER_OF_DONE_TASKS}/{TOTAL_NUMBER_OF_TASKS}:"
        )

    for task in TASK_TITLE:
        print(f"\t {task}")


if __name__ == "__main__":
    request_data()
