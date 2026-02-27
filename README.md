# Todo List React

A simple and clean Todo List app built with React and Vite.

## Features

- Add tasks
- Delete tasks
- Move tasks up and down
- Persist tasks with `localStorage`
- Input trimming to avoid empty/whitespace-only tasks

## Tech Stack

- React 19
- Vite 7
- JavaScript (ES Modules)
- CSS

## Getting Started

### Prerequisites

- Node.js 18+ (recommended)
- npm

### Installation

```bash
npm install
```

### Run Development Server

```bash
npm run dev
```

Then open the local URL shown in your terminal (usually `http://localhost:5173`).

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Create production build
- `npm run preview` - Preview production build locally
- `npm run lint` - Run ESLint

## Project Structure

```text
src/
  App.jsx
  ToDoList.jsx
  App.css
  index.css
  main.jsx
  utils/
    localStorage.js
```

## localStorage Notes

Tasks are saved under the key `tasks`.

- On app load, data is read from `localStorage`
- Data is validated with `Array.isArray(...)` before use
- On each tasks update, the latest list is written back to `localStorage`

## Future Improvements

- Use object-based tasks (`{ id, text }`) for stable keys
- Add edit task support
- Add completed state and filters (All/Active/Completed)
- Add unit/component tests

## License

This project is for learning and personal use.
