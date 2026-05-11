<h1 align="center">Terminal-Based Todo App</h1>

<p align="center">
  A command-line TODO application with PostgreSQL persistence, Rich TUI, user authentication, and a custom-built ORM — no Django, no SQLAlchemy.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-3776AB?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/PostgreSQL-Database-336791?style=flat-square&logo=postgresql&logoColor=white">
  <img src="https://img.shields.io/badge/Rich-Terminal%20UI-000000?style=flat-square">
  <img src="https://img.shields.io/badge/bcrypt-Auth-4A90E2?style=flat-square">
</p>

---

## Highlights

- **Custom ORM** — raw SQL with psycopg2, no external ORM framework
- **Rich TUI** — colorful, interactive terminal interface using the `rich` library
- **Auth** — bcrypt password hashing with per-user task isolation
- **Clean architecture** — models, ORM, and page components are properly separated

---

## Setup

**1. Clone**

```bash
git clone https://github.com/samandar-hamrayev/terminal-based-todo-app.git
cd terminal-based-todo-app
```

**2. Install dependencies**

```bash
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

**3. Configure database**

Copy `.env.example` to `.env` and fill in your PostgreSQL credentials:

```env
DB_HOST=localhost
DB_NAME=todo_db
DB_USER=your_user
DB_PASSWORD=your_password
```

**4. Run**

```bash
python main.py
```

---

## Project Structure

```
terminal-based-todo-app/
├── main.py       # Entry point
├── models/       # Data model definitions
├── orm/          # Custom SQL ORM layer
├── pages/        # TUI screen components
├── utils.py      # Shared helpers
└── .env.example
```

---

## Tech Stack

| Dependency | Purpose |
|------------|---------|
| `psycopg2` | PostgreSQL driver |
| `rich` | Terminal UI rendering |
| `bcrypt` | Password hashing |
| `python-dotenv` | Environment config |

---

## License

MIT
