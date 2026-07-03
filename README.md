# python-teams

A **Flask collaborative platform** — accounts, real-time messaging, shared projects, and calendars. A Pythonic take on the features found in Teams, Replit, and similar tools.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-SocketIO-000000?style=flat-square&logo=flask&logoColor=white)

## Features

- User registration and authentication
- **Socket.IO** real-time chat
- Contacts and messaging pages
- Shared project workspaces (`ProjectFiles/`)
- Calendar and deadline views
- Separate SQLite databases for users, chats, and contacts

## Tech stack

| Layer | Choice |
|-------|--------|
| Backend | Flask, Flask-SocketIO, Flask-Session |
| Auth | Werkzeug password hashing |
| DB | SQLite (multiple DB files) |
| Frontend | Jinja2 templates |

## Quick start

```bash
pip3 install -r requirements.txt
python3 app.py
```

Open **http://127.0.0.1:5000**

### IPv6 / LAN access

To bind on all interfaces for device testing, configure the host in `app.py` (see README screenshots for network setup notes).

## Project layout

```
app.py           # Main Flask + SocketIO app
helpers.py       # DB helpers
requirements.txt
templates/       # Home, messaging, projects, calendar
ProjectFiles/    # Shared project storage
screenshots/     # Feature walkthrough images
```

## Contributing

Open for contributions — messaging, project sync, and calendar integrations are active areas.

---

[malimba](https://github.com/malimba)
