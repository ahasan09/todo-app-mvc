# Todo App (MVC)

A vanilla JavaScript Todo application built using the Model-View-Controller (MVC) architectural pattern. Demonstrates clean separation of concerns without any frameworks.

## Features

- Add, edit, and delete todos
- Mark todos as done
- Filter by status (All / Done / Pending)
- Search todos
- Data persisted in `localStorage`

## Running

No installation needed. Open the entry point in any modern browser:

```bash
# macOS
open view/index.html

# Linux
xdg-open view/index.html

# Windows
start view/index.html
```

Or serve locally:

```bash
npx serve .
```

Then navigate to the `view/` folder in the browser.

## Prerequisites

- Any modern web browser (Chrome, Firefox, Edge, Safari)

## Project Structure

```
todo-app-mvc/
├── view/                       # HTML templates
├── controller/                 # Controller — handles user actions
├── model/                      # Model — data and business logic
├── local-storage-factory.js    # localStorage abstraction
├── enum/                       # Status enumerations
├── js/                         # Shared utilities
└── css/                        # Styles
```
