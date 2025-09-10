# video_portal_server

Backend service for a **video portal** built with **NestJS** and **TypeScript**.
It provides RESTful APIs for authentication, video management, and database access using **Prisma**.
The project also supports video processing with ffmpeg and email notifications via Nodemailer.

---

## 🚀 Installation

```bash
git clone https://github.com/Timson4eg/video_portal_server.git
cd video_portal_server
npm install
# or
bun install
```

---

## ⚙️ Environment Variables

Create a `.env` file in the project root with the following values:

```env
DATABASE_URL="postgresql://user:password@localhost:5432/mydb"
JWT_SECRET=your_secret
PORT=3000

# Email
SMTP_SERVER=smtp.mailgun.org
SMTP_LOGIN=your@email.com
SMTP_PASSWORD=your_password

# reCAPTCHA
RECAPTCHA_SECRET_KEY=your_recaptcha_key
```

_(keep `.env` out of version control; commit an `.env.example` if needed)_

---

## 📡 Available Scripts

From `package.json`:

```bash
npm run start:dev   # start app in watch mode
npm run build       # build for production
npm run start:prod  # run compiled app
npm run lint        # run eslint
npm run format      # run prettier
npm run test        # run unit tests
npm run test:e2e    # run end-to-end tests
npm run test:cov    # test coverage report
npm run db:reset    # reset database (destructive)
npm run seed:run    # seed database with test data
```

---

## 💾 Database (Prisma + PostgreSQL)

This project uses **Prisma ORM** with PostgreSQL.

```bash
# apply migrations
npx prisma migrate dev

# generate prisma client
npx prisma generate

# reset database & seed
npm run db:reset
npm run seed:run
```

---

## 📖 API Reference

_(example endpoints — adjust to your actual routes)_

| Method | Endpoint      | Description        |
| ------ | ------------- | ------------------ |
| GET    | `/videos`     | Get all videos     |
| POST   | `/videos`     | Upload new video   |
| GET    | `/videos/:id` | Get video by ID    |
| DELETE | `/videos/:id` | Delete video by ID |

---

## 🧪 Testing

The project uses **Jest** for unit and e2e tests.

```bash
npm run test       # run unit tests
npm run test:e2e   # run end-to-end tests
npm run test:cov   # generate coverage report
```
