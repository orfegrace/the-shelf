<img width="1440" height="709" alt="Screenshot 2026-06-13 at 11 31 02 PM" src="https://github.com/user-attachments/assets/d6632da3-bd0a-49a6-83a8-3e31b0317187" /># The Shelf 📚🏠

A personal tracker I built to keep my books and movies in one place. You can log entries, rate them, add notes, and view your library in a bunch of different ways.

---

## Screenshots of the website

### Library — Gallery View
<img width="1431" height="713" alt="Screenshot 2026-06-13 at 11 29 24 PM" src="https://github.com/user-attachments/assets/49d25e8b-1f5b-4559-a676-636eca2c5b11" />

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

Everything lives in a single index.html file. 
The top bar lets you navigate between three pages — Library, Stats, and Favorites. 
The Library has a search bar and 
five view options: gallery, table, timeline, board, and list. 
The right sidebar is for profile editing. 

---

## Note on data

Entry data lives in `localStorage` under your Supabase user ID — nothing gets saved to the database itself. Supabase only handles login. If you clear your browser storage, your entries will be gone.

---

*Made by Grace Chang*
