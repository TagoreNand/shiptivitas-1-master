# Shiptivitas-1

A kanban board for managing shipping requests. Built for the InsideSherpa Y Combinator training program.

## What it does

This is a React app that lets you drag shipping request cards between three columns: Backlog, In-Progress, and Complete. Cards change color when you move them between columns.

## Setup

```bash
git clone https://github.com/TagoreNand/shiptivitas-1-master.git
cd shiptivitas-1-master
npm install
npm start
```

Open http://localhost:3000 in your browser.

## The Task

This was part of an InsideSherpa virtual internship. The goal was to:

- Add drag-and-drop functionality to move cards between swimlanes
- Make cards change color based on their status
- Keep everything working on the frontend only (no backend needed)

## How it works

The app loads some sample shipping requests in `Board.js`. Each request looks like this:

```javascript
{
  id: 1,
  name: "Client Name",
  description: "What needs to be shipped",
  status: "backlog" // or "in-progress" or "complete"
}
```

Uses [Dragula](https://github.com/bevacqua/dragula) for the drag-and-drop stuff:

```javascript
import Dragula from 'dragula';
// Then use it to make containers draggable
```

## Project structure

```
src/
├── Board.js          # Main kanban board
├── App.js            # Root component
└── index.js          # Entry point
```

## Requirements met

- ✓ All requests start in backlog
- ✓ Three swimlanes (backlog, in-progress, complete)
- ✓ Drag cards up/down and between lanes
- ✓ Cards stay where you drop them
- ✓ Card colors change when moved between lanes

## Scripts

- `npm start` - Run development server
- `npm test` - Run tests
- `npm run build` - Build for production

## Links

- [InsideSherpa Module](https://www.insidesherpa.com/modules/oRMogWRHeewqHzA7u/58dLdeDgbwf9Ste3j)
- [Y Combinator Program](https://www.insidesherpa.com/virtual-internships/prototype/oRMogWRHeewqHzA7u/College%20Students%3A%20Learn%20how%20to%20work%20at%20a%20YC%20startup)
- [Dragula docs](https://github.com/bevacqua/dragula)

That's it. Pretty straightforward kanban board with drag-and-drop.
