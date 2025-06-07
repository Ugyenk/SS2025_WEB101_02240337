# Todo App with Zustand

A simple todo list app built with React and Zustand for easy state management.

## What it does

- Add new todos
- Mark todos as done/undone
- Delete todos
- Clear all completed todos
- Saves your todos automatically

## Getting Started

1. **Create the project**
   ```bash
   npx create-vite@latest my-todo-app
   cd my-todo-app
   ```

2. **Install Zustand**
   ```bash
   npm install zustand
   ```

3. **Start coding!**
   ```bash
   npm run dev
   ```

## How to build it

### 1. Create the store (src/store/todoStore.js)

```javascript
import { create } from 'zustand'

const useTodoStore = create((set) => ({
  todos: [],
  
  addTodo: (text) => set((state) => ({
    todos: [...state.todos, { 
      id: Date.now(), 
      text, 
      completed: false 
    }]
  })),
  
  toggleTodo: (id) => set((state) => ({
    todos: state.todos.map(todo =>
      todo.id === id ? { ...todo, completed: !todo.completed } : todo
    )
  })),
  
  removeTodo: (id) => set((state) => ({
    todos: state.todos.filter(todo => todo.id !== id)
  }))
}))

export default useTodoStore
```

### 2. Use it in your components

```javascript
import useTodoStore from './store/todoStore'

function TodoApp() {
  const { todos, addTodo, toggleTodo, removeTodo } = useTodoStore()
  
  // Your component logic here
}
```

## Why Zustand?

- Super simple to use
- No complicated setup
- Components only update when they need to
- Tiny file size
- Works great with React

## That's it!

Your todos will be ready to go. Add some styling and you're done!