# FeelFree
# 🕊️ FeelFree

**FeelFree** is a personal digital companion that blends emotion, productivity, and creativity — designed to help users **express their thoughts, manage reminders, and track income & expenses** in one comforting digital space.

This project recreates the nostalgic experience of writing in a **real diary**, complete with animations, a book-like interface, and interactive pencil cursor, using only **HTML, CSS, JavaScript, and SQL**.

---

## 🌸 Project Overview

**FeelFree** provides a calm and private environment where users can:
- Write their **daily diary entries** 📝  
- Set **reminders or alarms** ⏰ that ring until stopped  
- Track **income and expenses** 💰  

The interface mimics an **open book**, bringing a sense of comfort and creativity. The landing page features a **closed diary**, and clicking on it (with a pencil cursor) triggers an **animation of the book opening**, revealing the main dashboard inside.

---

## ✨ Key Features

### 📝 Diary
- Write, edit, and delete personal diary entries.  
- Auto-save entries with date and time.  
- Option to tag daily **moods** (😊 😞 😡 etc.).  
- Secure storage using SQL database.

### ⏰ Reminders / Alarms
- Create and manage reminders for important tasks or routines.  
- Custom **alarm sound** rings continuously until stopped.  
- Snooze and delete functionalities included.  
- Stored persistently in SQL.

### 💰 Income & Expense Tracker
- Add **income and expense records** with date and category.  
- Display **summary dashboard** showing total income, expenses, and current balance.  
- Optional future integration for data visualization using JS charts.

---

## 🎨 Design & Aesthetic

- **Theme:** Calm, paper-like textures with soft pastel tones.  
- **Cursor:** Hidden; replaced by a **pencil icon** for an authentic diary-writing effect.  
- **Animation:**  
  - Landing page shows a **closed diary/book**.  
  - On click, book **opens smoothly** into the main interactive page.  
- **Book Interface:** Each “page” represents a module (Diary / Reminders / Expenses).  
- **Font Style:** Ink-like handwritten fonts to simulate real handwriting.  

---

## 🧱 Page Structure

| Page | Description |
|------|--------------|
| `index.html` | Landing page with closed book animation and pencil cursor. |
| `home.html` | Main dashboard showing the open book interface. |
| `diary.html` | Daily diary entry page. |
| `reminders.html` | Reminder/alarm setup and management page. |
| `finance.html` | Income & expense tracking page. |
| `settings.html` | Manage theme, alarm sound, and reset data. |
| `about.html`  | Information about FeelFree and credits. |
| `login.html` / `register.html`  | For user authentication, if implemented later. |

---

## 🗄️ Database Schema (SQL)

### Table: `diary_entries`
| Column | Type | Description |
|---------|------|-------------|
| id | INT (PK) | Unique entry ID |
| date | DATE | Date of entry |
| content | TEXT | Diary content |
| mood | VARCHAR | Mood tag |

### Table: `reminders`
| Column | Type | Description |
|---------|------|-------------|
| id | INT (PK) | Reminder ID |
| title | VARCHAR | Reminder title |
| time | DATETIME | Scheduled time |
| active | BOOLEAN | Status of reminder |

### Table: `transactions`
| Column | Type | Description |
|---------|------|-------------|
| id | INT (PK) | Transaction ID |
| type | ENUM('income', 'expense') | Type of transaction |
| amount | FLOAT | Amount value |
| category | VARCHAR | Category (e.g., Food, Study, etc.) |
| date | DATE | Date of transaction |
| note | TEXT | Additional notes |

---

## 💻 Tech Stack

| Category | Technology |
|-----------|-------------|
| **Frontend** | HTML, CSS, JavaScript |
| **Backend** | JavaScript (with SQL integration or Node.js optional) |
| **Database** | SQL (MySQL / SQLite) |
| **UI Elements** | CSS animations, Canvas, HTML Audio API |

---

## 🌱 Future Enhancements

- Daily motivational quotes section.  
- Calendar view for diary entries.  
- Export diary data as PDF or TXT.  
- Dark/Night writing mode.  
- Voice note feature for diary.  
- User authentication (login/register).  

---

## 💡 Purpose

FeelFree was created to help users **release emotions, stay organized, and maintain mindfulness** in a comforting virtual environment — a balance of **art, memory, and technology**.

---

## 👨‍💻 Developer

**Developed by:** Chandan  
**Project Type:** Mini Project  
**Tech Stack:** HTML, CSS, JavaScript, SQL  
**Status:** In Development  
**Year:** 2025  

---

## 🖼️ Preview (Concept)

> “A diary that opens when you click with your pencil.  
> Inside, you’ll find not just words — but a reflection of your daily life.”
