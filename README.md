# Quick Notes

A lightweight, client-side note-taking web application built with vanilla HTML, CSS, and JavaScript. Quick Notes lets you create, edit, and delete notes directly in the browser with instant persistence via `localStorage` and a built-in dark/light theme toggle.

## Features

- **Full CRUD Functionality:** Create new notes, edit existing entries in-place, and delete notes with instant DOM updates.
- **Persistent Local Storage:** Automatically syncs both your notes array (`quickNotes`) and your active theme preference (`theme`) to `localStorage` so data persists across page reloads.
- **Dark & Light Theme:** Toggle between light and dark color schemes on the fly using CSS custom properties (`:root` and `.dark-theme`)[cite: 1, 3].
- **Native Modal Dialogs:** Uses the HTML5 `<dialog>` API for the note creation/editing interface, including backdrop blur and click-outside-to-close support[cite: 1, 2, 3].
- **Responsive Grid Layout:** Auto-adjusting card grid (`repeat(auto-fill, minmax(300px, 1fr))`) with smooth hover actions and an empty-state fallback prompt when no notes exist[cite: 1, 3].
- **Zero Dependencies:** Pure vanilla stack—no frameworks, build tools, or external runtime libraries required[cite: 1, 2, 3].

## Tech Stack

- **Markup:** HTML5 (Semantic elements, `<dialog>` modal API)
- **Styling:** CSS3 (CSS Variables, CSS Grid, Flexbox, `backdrop-filter`, Google Fonts - *Poppins*)[cite: 3]
- **Logic:** Vanilla JavaScript (ES6+, DOM manipulation, `localStorage` API)

## Project Structure

```text
├── index.html   # App layout, header controls, notes grid container, and <dialog> form[cite: 2]
├── style.css    # Theme variables, responsive grid styling, card hover states, and modal styles[cite: 3]
└── app.js       # State management, CRUD handlers, localStorage sync, and theme toggling
