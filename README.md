# The Shelf

A personal tracker I built to keep my books and movies in one place. You can log entries, rate them, add notes, and view your library in a bunch of different ways.

---

## Screenshots of the website

### Library — Gallery View (7 views, search bars, condition drop downs)
<img width="1440" height="748" alt="Screenshot 2026-06-28 at 11 55 50 PM" src="https://github.com/user-attachments/assets/3680863e-8023-4b12-b703-39abb845a389" />

### Library — Board View
<img width="1440" height="744" alt="Screenshot 2026-06-14 at 11 18 18 AM" src="https://github.com/user-attachments/assets/bfc5800b-9752-4fe4-aba1-d92567306c81" />

### Library - Spine View 
<img width="1440" height="749" alt="Screenshot 2026-06-28 at 11 57 08 PM" src="https://github.com/user-attachments/assets/2c74aae8-5a0b-48bd-a3e7-8aa3e4c41b98" />

### Library - Adding an Entry
<img width="1440" height="715" alt="Screenshot 2026-06-14 at 11 10 20 AM" src="https://github.com/user-attachments/assets/fb950260-b9dc-4b1a-8dab-fdbea0d56585" />

### Library - Entry card view (Click on the title to search on Google)
<img width="1440" height="710" alt="Screenshot 2026-06-15 at 11 41 54 AM" src="https://github.com/user-attachments/assets/a92ef7fa-be9b-40bd-8a00-333c9360e1f0" />

### Stats
<img width="1440" height="753" alt="Screenshot 2026-06-14 at 11 36 46 AM" src="https://github.com/user-attachments/assets/aba7d709-7ac1-49e3-b5c5-97f13ced33d9" />

### Favorites
<img width="1440" height="709" alt="Screenshot 2026-06-13 at 11 31 02 PM" src="https://github.com/user-attachments/assets/88373572-9dbf-473d-a7a8-124a2d48e97c" />


---

## What it does

- Log movies and books together in one library
- Mark things as Finished, In Progress, Did Not Finish, or Not Started
- Rate entries 1–5 stars
- Add a cover image URL, genre, director/author, and personal notes
- Switch between 5 views: Gallery, Table, Timeline, Board, and List
- Board can be grouped by Rating, Genre, or Year Wached/Read
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
| Database | [Supabase](https://supabase.com) (entries synced per user) |

---

## Setup

1. Clone the repo
3. Create the database table
4. Open it! No build step needed — just open `index.html` in your browser. Or deploy to GitHub Pages, Vercel, or Netlify.

---

## Project structure

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
        ├── List View
│       ├── Spine View
│       └── Mood Board View
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


*Made by orfegrace*
