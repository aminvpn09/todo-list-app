# To-Do List Application

A modern, feature-rich to-do list application with local storage functionality. Built with vanilla HTML, CSS, and JavaScript.

## Features

✅ **Add Tasks** - Easily add new tasks with a simple input field

✅ **Mark Complete** - Check off tasks as you complete them

✅ **Delete Tasks** - Remove individual tasks or clear all completed tasks

✅ **Filter Tasks** - View all tasks, only active tasks, or only completed tasks

✅ **Local Storage** - All tasks are automatically saved to your browser's local storage

✅ **Persistent Data** - Your tasks remain even after closing and reopening the browser

✅ **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices

✅ **Task Statistics** - See how many tasks you have remaining

## Installation

1. Clone the repository:
```bash
git clone https://github.com/aminvpn09/todo-list-app.git
cd todo-list-app
```

2. Open `index.html` in your web browser or use a live server:
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server
```

3. Visit `http://localhost:8000` in your browser

## Usage

### Adding a Task
1. Type your task in the input field
2. Press Enter or click the "Add" button
3. The task will appear in the list below

### Completing a Task
1. Click the checkbox next to a task to mark it as complete
2. Completed tasks will appear with a strikethrough

### Deleting a Task
1. Click the "Delete" button next to a task to remove it
2. Click "Clear Completed" to remove all completed tasks at once

### Filtering Tasks
- **All** - View all tasks
- **Active** - View only incomplete tasks
- **Completed** - View only completed tasks

## How Local Storage Works

This application uses the browser's `localStorage` API to persistently save your tasks. Here's how it works:

- Each task is stored as a JavaScript object with:
  - `id`: Unique identifier (timestamp)
  - `text`: The task description
  - `completed`: Boolean status
  - `createdAt`: Timestamp of creation

- All tasks are saved as a JSON array in localStorage
- Whenever you add, complete, or delete a task, the changes are automatically saved
- When you refresh the page or close the browser, your tasks are restored from localStorage

### Clearing Local Storage

To clear all tasks and reset the application:
1. Open your browser's Developer Tools (F12 or Right-click → Inspect)
2. Go to the "Application" or "Storage" tab
3. Find "Local Storage" and select your domain
4. Look for the key `todoList` and delete it
5. Refresh the page

## File Structure

```
todo-list-app/
├── index.html      # HTML structure
├── styles.css      # Styling and responsive design
├── script.js       # JavaScript logic and local storage handling
└── README.md       # Documentation
```

## Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Flexbox layout, animations, responsive design
- **Vanilla JavaScript** - No frameworks or dependencies
- **Local Storage API** - Browser-based data persistence

## Browser Compatibility

Works on all modern browsers that support:
- ES6 JavaScript
- LocalStorage API
- CSS Flexbox

Tested on:
- Chrome/Chromium (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Future Enhancements

- [ ] Due dates and reminders
- [ ] Task categories/tags
- [ ] Priority levels
- [ ] Dark mode
- [ ] Drag and drop to reorder tasks
- [ ] Export/Import functionality
- [ ] Cloud sync with backend server

## Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Author

Created with ❤️ by [aminvpn09](https://github.com/aminvpn09)
