# TodoList

A simple WPF desktop application for managing tasks, built with C# and .NET 10.

![Platform](https://img.shields.io/badge/platform-Windows-blue) ![Framework](https://img.shields.io/badge/.NET-10.0-purple) ![UI](https://img.shields.io/badge/UI-WPF-blueviolet)

## Features

- Add, edit, and delete tasks
- Mark tasks as completed by clicking the circle icon
- Double-click a task to open the edit window
- Each task has a title, description, due date, and completion status
- Export tasks to XML and reload them on next launch
- Material Design inspired UI with blue accent colors

## Project Structure

```
TodoList/
├── TodoList.csproj
├── App.xaml
├── App.xaml.cs
├── Properties/
│   └── AssemblyInfo.cs
├── TodoTask.cs
├── TaskListWindow.xaml
├── TaskListWindow.xaml.cs
├── TaskEditWindow.xaml
└── TaskEditWindow.xaml.cs
```

## Requirements

- Windows 10 or later
- [.NET 10 SDK](https://dotnet.microsoft.com/download)
- Visual Studio 2022 or later (with .NET desktop development workload)

## Getting Started

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/TodoList.git
   ```
2. Open `TodoList.csproj` in Visual Studio
3. Press **F5** to build and run

## Data Persistence

Tasks are saved to `Tasks.xml` in the application output directory (`bin/Debug/net10.0-windows/`).

- **Export** — saves the current task list to `Tasks.xml`
- **Reload** — loads tasks from `Tasks.xml`, discarding unsaved changes

## Usage

| Action | How |
|---|---|
| Add task | Click **Add** |
| Edit task | Select task and click **Edit**, or double-click the task |
| Delete task | Select task and click **Delete** |
| Toggle completed | Click the circle icon on the left of the task |
| Save tasks | Click **Export** |
| Reload tasks | Click **Reload** |

