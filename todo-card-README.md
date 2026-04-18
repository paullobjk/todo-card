# Todo Item Card — HNG Frontend Stage 0

A high-fidelity, interactive Task Card component built with semantic HTML, CSS, and vanilla JavaScript.

---

## Live URL

> **https://YOUR-DEPLOYED-URL**

---

## How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/todo-card.git
   cd todo-card
   ```

2. Open `index.html` directly in your browser — no build step needed:
   ```bash
   open index.html
   ```

   Or use a simple local server:
   ```bash
   npx serve .
   ```

---

## Decisions Made

- **Vanilla HTML/CSS/JS** — No framework needed for a single card component. Keeps it lightweight and fast.
- **Semantic HTML** — Used `<article>` as the card root, `<h2>` for the title, `<p>` for description, `<time>` elements with `datetime` attributes for dates, `<ul>/<li>` for tags, and `<button>` for actions.
- **Real checkbox** — Used a native `<input type="checkbox">` with a linked `<label>` for accessibility.
- **Dynamic time** — The due date is set 5 days from the current time. The "time remaining" string updates every 45 seconds using `setInterval` and reflects the real current time accurately.
- **Dark theme** — Chosen for the "startup productivity app" energy requested in the brief. High contrast, clean, and professional.
- **CSS custom properties** — All colors and spacing defined as variables for easy theming.

---

## Trade-offs

- **No framework** — React or Vue would add unnecessary complexity for a single card. Vanilla JS is sufficient and performs better.
- **Inline JS** — Kept in the HTML file for simplicity and single-file deployability.
- **Static task data** — The card uses hardcoded demo data since no API or state management was required by the brief.

---

## Test IDs Implemented

| Element | data-testid |
|---------|-------------|
| Card container | `test-todo-card` |
| Title | `test-todo-title` |
| Description | `test-todo-description` |
| Priority badge | `test-todo-priority` |
| Due date | `test-todo-due-date` |
| Time remaining | `test-todo-time-remaining` |
| Status indicator | `test-todo-status` |
| Checkbox | `test-todo-complete-toggle` |
| Tags list | `test-todo-tags` |
| Tag: Design | `test-todo-tag-design` |
| Tag: UX | `test-todo-tag-ux` |
| Tag: Frontend | `test-todo-tag-frontend` |
| Tag: Q2 Sprint | `test-todo-tag-q2` |
| Edit button | `test-todo-edit-button` |
| Delete button | `test-todo-delete-button` |
