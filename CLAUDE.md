# JS-ToDo-App

Vanilla JavaScript to-do application with a structured MVC-like pattern, supporting task creation, editing, deletion, filtering, search, and localStorage persistence.

## Tech Stack
- Vanilla JavaScript (ES5, modular IIFE pattern)
- HTML5 / CSS3
- No frameworks or build tools

## Project Structure
```
JS-ToDo-App/
  view/
    index.html                  # Main entry point
  js/
    enum/todo-enum.js
    model/
      view.js                   # DOM element references
      validation-factory.js
      todo-modal-factory.js
      todo-app-factory.js       # Core app data/logic
    controller/todo-controller.js
    local-storage-factory.js
  css/app.css
  other/                        # Earlier single-file prototype
```

## Development
No dependencies to install. Open `view/index.html` in a browser:
```bash
open JS-ToDo-App/view/index.html
# or serve with:
python3 -m http.server 8080
```

## Key Notes
- Evolved version of Hasan-ToDo-App with cleaner separation of concerns across multiple JS modules loaded via `<script>` tags.
- All modules attach to a global `window.ToDoApp` namespace.
- `other/` contains the original single-file prototype and is not active code.
