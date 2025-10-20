# Neon Todo List

A modern, glassy, and futuristic Todo List web application with category and priority tagging, localStorage persistence, and a stylish dark/light UI toggle.

---

Project title
- Neon Todo List

Summary
- A lightweight, client-side Todo List app that lets users add tasks with a category and priority, mark tasks as completed (or undo), delete tasks, and persist data across sessions using localStorage. The UI has been updated to a modern, glassy, neon-inspired look with a responsive layout and a dark mode option.

Key features
- Glassy, futuristic UI with soft shadows, blur, and neon gradients
- Add tasks with:
  - Task text
  - Category (Work, Personal, Shopping, Other)
  - Priority (High, Medium, Low)
- Complete/Undo and Delete actions per task
- LocalStorage persistence for tasks and dark-mode state
- Dark mode styling with neon glow and glass panels
- Responsive layout for mobile and desktop

Setup instructions
- Open the index.html file in any modern web browser (no server required).
- Optionally host on GitHub Pages for easy sharing.

Usage instructions
- Type a task in the input field.
- Select a category and a priority.
- Click Add Task to save.
- Use Complete to toggle completion (Undo when completed).
- Use Delete to remove a task.
- Toggle dark mode with the top-right button to switch to a neon-dark aesthetic.

Technical details
- HTML structure:
  - Header with a glassy container
  - Task form (id="task-form") with inputs for task, category, priority, and a submit button
  - Task list (ul id="task-list") where each task renders as a glass card
- CSS structure:
  - Global theme variables and a neon-inspired color system
  - Glassy card styling for tasks
  - Responsive grid for the form
  - Dark mode styling via the class on body (dark-mode)
- JavaScript structure:
  - Tasks are stored in an array and persisted to localStorage under the key 'tasks'
  - Functions: renderTasks, updateLocalStorage, addTask, completeTask, deleteTask
  - Event listeners for form submission, task actions, and dark mode toggle
  - On load, initialize tasks from localStorage and apply dark mode if set

Changes made in Round 2
- Replaced the previous, basic UI with a neon-glass, futuristic design:
  - Added a gradient, glass-like container with blur and soft borders
  - Implemented a neon gradient Add Task button and neon-task actions
  - Reworked task items to be card-style with a two-column layout: content and actions
  - Introduced a subtle animated background glow for a futuristic vibe
  - Enhanced dark mode visuals with neon accents and glass panels
  - Updated responsive behavior to stack the form on small screens while keeping a clean layout
  - Improved accessibility with ARIA labels and semantic structure
  - Maintained existing functionality (add, complete/undo, delete, localStorage)

Deployment info (GitHub Pages)
- Steps to publish:
  - Push the repository to GitHub
  - Go to the repository Settings > Pages
  - Select main branch (or a docs folder) as source
  - Save and wait for GitHub Pages to update the site
- Ensure index.html is at the root (or configured path) for GitHub Pages to serve it.

License
- MIT

Notes
- The app remains fully client-side. No server is required.
- You can customize colors by tweaking CSS variables in the <style> block for future branding.
- If you want to add more categories or features (e.g., due dates, filters), the structure supports easy extension.