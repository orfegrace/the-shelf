# The Shelf

A personal tracker I built to keep my books and movies in one place. You can log entries, rate them, add notes, and view your library in a bunch of different ways.

---

## Screenshots of the website

### Library — Gallery View
<img width="1440" height="715" alt="Screenshot 2026-06-14 at 10 49 35 AM" src="https://github.com/user-attachments/assets/65c6fb65-66fd-4b15-9345-1d31c51e7c4e" />

### Library — Board View
<img width="1440" height="715" alt="Screenshot 2026-06-13 at 11 29 52 PM" src="https://github.com/user-attachments/assets/5e461ddb-cca8-4424-ae57-a2576dfe58a6" />

### Library - Stats
<img width="1440" height="714" alt="Screenshot 2026-06-13 at 11 49 26 PM" src="https://github.com/user-attachments/assets/44348f9d-5992-43b3-8b87-295094421054" />


### Favorites
<img width="1440" height="709" alt="Screenshot 2026-06-13 at 11 31 02 PM" src="https://github.com/user-attachments/assets/88373572-9dbf-473d-a7a8-124a2d48e97c" />


---

## What it does

- Log movies and books together in one library
- Mark things as Finished, In Progress, Did Not Finish, or Not Started
- Rate entries 1–5 stars
- Add a cover image URL, genre, director/author, and personal notes
- Switch between 5 views: Gallery, Table, Timeline, Board, and List
- Board can be grouped by Rating, Genre, or Year Added
- Favorites page auto-collects anything rated 4★ or above
- Stats page shows your totals, average rating, top genre, and charts
- Search and filter by type, status, rating, or sort order
- Login with email and password — each account's data is stored separately

---

## Built with

| | |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript |
| Auth | [Supabase](https://supabase.com) |
| Charts | [Chart.js v4](https://www.chartjs.org/) |
| Fonts | Baloo 2 + Plus Jakarta Sans |
| Storage | `localStorage` (per user ID) |

---

## Setup

### 1. Clone the repo

```bash
git clone https://github.com/grace-chang/the-shelf.git
cd the-shelf
```

### 2. Add your Supabase credentials

Create a project at [supabase.com](https://supabase.com), then open `index.html` and replace these two lines near the bottom:

```js
const SUPABASE_URL = 'YOUR_SUPABASE_PROJECT_URL';
const SUPABASE_KEY = 'YOUR_SUPABASE_ANON_KEY';
```

### 3. Open it

No build step needed — just open `index.html` in your browser. Or deploy to GitHub Pages, Vercel, or Netlify.

---

## Project structure

## Project Structure

Everything is built inside a single `index.html` file.

```text id="11ekfq"
index.html
├── Top Navigation Bar
│   ├── Library
│   ├── Stats
│   └── Favorites
│
├── Library Page
│   ├── Search Bar
│   └── View Options
│       ├── Gallery View
│       ├── Table View
│       ├── Timeline View
│       ├── Board View
│       │   ├── Rating
│       │   ├── Genre
│       │   └── Year Added
│       └── List View
│
├── Stats Page
│   └── Displays collection-related statistics
│
├── Favorites Page
│   └── Shows saved or favorited items
│
└── Right Sidebar
    └── Profile Editing Panel
```

---

## Note on data

Entry data lives in `localStorage` under your Supabase user ID — nothing gets saved to the database itself. Supabase only handles login. If you clear your browser storage, your entries will be gone.

---

*Made by Grace Chang*
