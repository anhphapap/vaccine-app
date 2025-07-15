# 💉 Vaccination Center

A full-stack mobile-based application for managing vaccination records, appointments, healthcare staff interactions, and real-time chat. This project is designed to streamline vaccination operations for citizens, medical staff, and administrators.

> Frontend & Realtime Chat: React Native & Firebase by [@anhphapap](https://github.com/anhphapap)  
>  Backend: Django by [@godreplyme](https://github.com/godreplyme)

---

## Features

### Users

- Register with personal information and upload a profile photo.
- View vaccination schedule and book appointments.
- Receive appointment reminders via **email**.
- Make purchases and payments through **VNPay**.
- Download **vaccination certificates**.
- View **vaccination history** by vaccine type.
- **Chat in real-time** with staff using Firebase.

### Staff

- Update vaccination status for each citizen.
- Add health notes and monitor post-vaccination reactions.
- View detailed vaccination history of each user.
- **Chat in real-time** with users using Firebase.

### Admins

- Manage user and medical staff accounts.
- Manage vaccine data (create / update / delete).
- Manage and track **community vaccination campaigns**.
- Access analytics:
  - Number of vaccinated users
  - Completion rate of vaccination schedules
  - Most-used vaccine types by **month**, **quarter**, and **year**

---

## Tech Stack

| Layer           | Technology                                  |
| --------------- | ------------------------------------------- |
| Mobile App      | React Native                                |
| UI Framework    | React Native wrapper                        |
| Backend         | Django + Django REST Framework              |
| Realtime Chat   | Firebase (Realtime Database)                |
| Payment         | VNPay Integration                           |
| Auth            | OAuth 2                                     |
| Scheduled Tasks | Redis + Celery (daily job processing)       |
| Email Service   | SendGrid (transactional + scheduled emails) |

---

## Getting Started

### Frontend (React Native)

```bash
cd frontend
npm install
npx expo start   # Or use npx react-native run-android
```

> Make sure you have Expo CLI or React Native environment installed.

---

### Backend (Django)

```bash
cd backend
python -m venv env
source env/bin/activate
pip install -r requirements.txt

# Set up the database
python manage.py migrate

# Start the development server
python manage.py runserver
```

---

## API Configuration

In your React Native app, set the base URL for API calls:

```js
const BASE_URL = "http://<your-local-ip>:8000/api/";
```

> ⚠️ If you're running the app on a real device, replace `localhost` with your machine’s local IP address.

---

## Contributors

| Name         | Role     | GitHub                                       |
| ------------ | -------- | -------------------------------------------- |
| Pham Anh Pha | Frontend | [@anhphapap](https://github.com/anhphapap)   |
| Nguyen Ho Vu | Backend  | [@godreplyme](https://github.com/godreplyme) |

---
