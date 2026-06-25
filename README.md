# LibraryManagementSystem

# Central Library — Library Management System

A simple web app to manage a college library. It handles the book catalog, student/member records, issuing and returning books, and fine calculation.

Built with plain **HTML, CSS, and JavaScript**. No installation, no server, no database setup needed.

---

## How to run it

1. Download the file `library-management-system.html`
2. Double-click it to open in any browser (Chrome, Edge, Firefox)
3. That's it. The app is ready to use.

You don't need internet, Node.js, or any software installed. It works completely offline.

---

## What it can do

### 1. Dashboard
Shows a quick summary: how many books are in the library, how many are available, how many are issued, how many are overdue, and how much fine is pending.

### 2. Books
- Add a new book (title, author, ISBN, category, number of copies)
- Edit or delete a book
- Search books by title, author, or ISBN
- Filter books by category
- Won't let you delete a book that is currently issued to someone

### 3. Members
- Add a new member (name, roll number, department, contact)
- Edit or delete a member
- Search members by name, roll number, or department
- Won't let you delete a member who still has a book issued

### 4. Issue / Return
- Issue a book to a member (loan period is automatically set to 14 days)
- Return a book — the app automatically calculates a fine if it's overdue
- **Fine rule: ₹5 per day after the due date**
- Shows a list of all books currently on loan, with their due dates

### 5. Transactions
- Full history of every book that was ever issued or returned
- Search and filter by status (issued / overdue / returned)

---

## Saving your data

All data is saved automatically in your browser (using `localStorage`). This means:
- Your data stays saved even after you close the browser
- The data is only stored on the computer you're using — it doesn't go to the internet

### Backup options (in the sidebar)
- **Export backup** — downloads all your data as a `.json` file. Keep this safe.
- **Import backup** — load data back from a `.json` backup file.
- **Reset demo data** — wipes everything and reloads the sample data the app came with. Useful before a demo or viva.

---

## Demo data

The app comes pre-loaded with sample books, members, and transactions (including one overdue book) so you can try it out right away without entering anything yourself.

---

## Tech used

| Part | Technology |
|------|------------|
| Structure | HTML5 |
| Styling | CSS3 (no framework) |
| Logic | JavaScript (vanilla, no framework or library) |
| Storage | Browser localStorage |

No React, no backend, no npm install. Everything lives in one HTML file, so it's easy to submit, email, or run on any lab computer.

---

## Project structure

```
library-management-system.html   ← the whole app (HTML + CSS + JS in one file)
```

---

## Good to know

- Works best on a laptop/desktop screen but is also responsive on tablets and phones.
- If you clear your browser's site data/cache, the saved library data will be lost — export a backup first if that matters to you.
- This is a front-end only project (no real server or database), which makes it ideal for a college mini-project or assignment, but not meant for production/real institutional use with many simultaneous users.
