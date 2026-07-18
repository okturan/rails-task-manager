# Rails Task Manager

> **Status:** completed Rails CRUD learning exercise from 2021. It is an educational application, not a maintained task-management product.

The application stores tasks with a title, details, and completion state. It provides list, show, create, edit, update, and delete flows through server-rendered Rails views.

## What it demonstrates

- A complete controller-level CRUD path.
- Active Record persistence backed by a `tasks` table.
- Strong parameters and shared record lookup.
- Reusable form partials and server-rendered views.
- A boolean completion state with a database default.

## Historical local setup

The lockfile targets Ruby 2.7.3 and Rails 6.0.4. This is a preserved historical toolchain with known dependency advisories, not a claim of current Rails support. If inspected, run it only in an isolated local environment; do not expose or deploy this dependency set.

```bash
bundle install
bin/rails db:setup
bin/rails server
```

Then open `http://localhost:3000/tasks`.

## Data model

```text
Task
├── title: string
├── details: text
└── completed: boolean (default: false)
```

The repository intentionally has no hosted demo, package, release stream, or active CI. Any future Rails or Ruby upgrade should be verified as a dedicated maintenance change rather than implied by this archive README.
