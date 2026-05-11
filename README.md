# Terminal-Based Todo App

A feature-rich command-line TODO application with a PostgreSQL backend, a beautiful terminal UI via **Rich**, user authentication, and a custom ORM layer built from scratch.

## Features

- Create, view, update, and delete tasks from the terminal
- **User authentication** with bcrypt password hashing
- **PostgreSQL** persistence
- **Rich** library for colorful, interactive terminal UI
- **Custom ORM** — no Django or SQLAlchemy
- Per-user task isolation

## Tech Stack

- Python 3.9+
- PostgreSQL + psycopg2
- Rich (terminal UI)
- bcrypt (password hashing)
- python-dotenv

## Setup

### 1. Clone

```bash
git clone https://github.com/samandar-hamrayev/terminal-based-todo-app.git
cd terminal-based-todo-app
```

### 2. Install dependencies

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### 3. Configure database

Create a `.env` file based on `.env.example`:

```env
DB_HOST=localhost
DB_NAME=todo_db
DB_USER=your_user
DB_PASSWORD=your_password
```

### 4. Run

```bash
python main.py
```

## Project Structure

```
terminal-based-todo-app/
├── main.py       # Entry point and main app loop
├── models/       # Data model definitions
├── orm/          # Custom database ORM layer
├── pages/        # TUI screen/page components
├── utils.py      # Shared utilities
└── .env.example
```

## License

MIT
