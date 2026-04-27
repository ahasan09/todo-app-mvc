# Improvement Plan: JS-ToDo-App

## Overview
More structured than Hasan-ToDo-App with a clear MVC separation, but still uses ES5, a global namespace pattern, and has no tests or build pipeline.

## Improvements

### Code Quality
- Convert to ES modules to eliminate the `window.ToDoApp` global namespace
- Migrate to TypeScript — define a `Task` interface and type all factories/controllers
- Add ESLint + Prettier
- Delete the `other/` prototype folder (dead code)

### Testing
- Add Jest unit tests for each factory (`todo-app-factory`, `validation-factory`, `local-storage-factory`)
- Add Playwright e2e tests for creating, editing, deleting, and filtering tasks

### Build Pipeline
- Add Vite for bundling, hot-reload dev server, and production build
- Add GitHub Actions CI for linting and testing

### Accessibility
- Add ARIA roles and labels to modal dialogs and form controls
- Ensure keyboard operability (close modal on Escape, focus management after open/close)

### Features
- Add subtasks / checklists inside a task
- Add due dates and sorting by due date
- Add task categories/labels with color coding
- Add export to JSON/CSV

### Architecture
- Consider replacing the manual MVC wiring with a lightweight reactive library (e.g., Preact or Solid.js) if complexity grows
