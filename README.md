# Employees Management System

A C# console app for managing a list of employees through a keyboard menu.

## Features

- **Keyboard menu:** move with the **Up** and **Down** arrow keys (or **Home** and **End**), press **Enter** to choose. The selected item is highlighted.
- **Add New Employee**, with validation:
  - **ID:** a whole number, not 0, and not already used by another employee
  - **Name:** can't be empty and can't contain digits
  - **Salary:** a number, not 0
- **Display Employees:** shows each employee's ID, name and salary. Names are shown with a capital first letter.
- **Sort Employees:** lists the employees in alphabetical order by name.
- **Exit:** choose Exit or press **Esc**, then confirm with **Y** or **N**.

Employees are kept in memory, so the list is cleared when the app closes.

## Project structure

| File | What it does |
|---|---|
| `Program.cs` | The menu: drawing it, highlighting and reading the keys |
| `Employees.cs` | The employee data, the employees list, and the add, display and sort features |

## Tech stack

- C#
- .NET Framework 4.7.2 console app
- LINQ (for checking IDs and sorting)

## How to run

You need Windows with Visual Studio and the .NET Framework 4.7.2 developer pack.

1. Open `EmployeesManagementSystem.sln` in Visual Studio.
2. Press **F5**.

Run it in a normal console window. The menu moves the cursor and changes colors, which some built-in terminals don't support.
