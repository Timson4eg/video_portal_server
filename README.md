# video_portal_server

Backend service for a video portal built with **NestJS** and **TypeScript**.
It provides RESTful APIs for video management, authentication, and database access using **Prisma**.
The project includes utilities for seeding data, video processing with ffmpeg, and email notifications.

---

## 📖 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Environment Variables](#-environment-variables)
- [Available Scripts](#-available-scripts)
- [Database](#-database)
- [API Reference](#-api-reference)
<!-- - [Testing](#-testing)
- [Author](#-author)
- [License](#-license) -->

---

## ✨ Features

- NestJS modular architecture
- PostgreSQL + Prisma ORM
- JWT authentication with Passport
- Video upload & processing (ffmpeg)
- Email sending with Nodemailer
- Google reCAPTCHA integration
- Seeder for test data

---

## 🛠 Tech Stack

- [NestJS](https://nestjs.com) — Node.js framework
- [Prisma](https://www.prisma.io) — ORM
- [PostgreSQL](https://www.postgresql.org) — database
- [Passport + JWT](http://www.passportjs.org) — authentication
- [Nodemailer](https://nodemailer.com) — email delivery
- [Fluent-ffmpeg](https://www.npmjs.com/package/fluent-ffmpeg) — video processing
- [Jest](https://jestjs.io) — testing framework

---

## 📦 Installation

```bash
# clone repo
git clone https://github.com/Timson4eg/video_portal_server.git

cd video_portal_server

# install dependencies
npm install
# or
bun install
```
