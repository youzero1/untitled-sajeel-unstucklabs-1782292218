---
status: pending
title: Todo App
---

1. Set up the global stylesheet at /app/src/styles/global.css with `@import "tailwindcss";` as the first line.

2. Set up /app/src/main.tsx to render the root App component and import the global stylesheet.

3. Create a shared TypeScript type at /app/src/types/todo.ts that defines a Todo item with: a unique id, a text string, and a completed boolean.

4. Create a custom hook at /app/src/hooks/useTodos.ts that manages the todo list state. It should expose: the list of todos, a function to add a new todo, a function to toggle a todo's completed status, and a function to delete a todo.

5. Create a reusable input + button component at /app/src/components/AddTodoForm.tsx. It renders a text input and an "Add" button side by side. It calls a provided callback with the new todo text when submitted (via button click or pressing Enter). It clears the input after submission.

6. Create a reusable component at /app/src/components/TodoItem.tsx that renders a single todo row. It shows a checkbox on the left (checked when completed), the todo text in the middle (with a strikethrough style when completed), and a delete (trash/×) button on the right.

7. Create a reusable component at /app/src/components/TodoList.tsx that receives the list of todos and renders a TodoItem for each one. If the list is empty, it shows a friendly empty-state message like "No tasks yet — add one above!".

8. Create the page component at /app/src/pages/TodoPage.tsx. It uses the useTodos hook and composes AddTodoForm and TodoList together. It also displays a summary line below the list showing how many tasks are remaining (e.g. "2 of 5 tasks remaining").

9. Update /app/src/App.tsx to render TodoPage as the main content of the app. The page should be centered on screen with a clean, minimal card layout.

10. Update /app/index.html to set a meaningful page title like "Todo App".
