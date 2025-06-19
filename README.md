# garagesalio
Here’s a complete `README.md` file for your **GarageSalio** GitHub repository, tailored to your MVP stack and local development workflow:

---

# 🚗 GarageSalio

**GarageSalio** is a web-based directory for discovering and posting local garage sales. It offers a clean map and list interface, plus social sign-in, listing creation, and reminders. Built as an MVP with Next.js, Express, PostgreSQL, and Docker.

---

## ✨ Features

- 🌐 Browse nearby garage sales on an interactive map
- 🔍 Search and filter by location, date, and keywords
- 📝 Post your own sale with title, images, and schedule
- 🔒 OAuth login with Google and Facebook (via Firebase Auth)
- 🗺 Location services + address autocomplete
- ⏰ Email reminders for upcoming sales
- 🛠 Admin tools to flag and manage listings

---

## 🧱 Tech Stack

| Layer         | Tech                            |
|---------------|---------------------------------|
| Frontend      | Next.js, React, Tailwind CSS    |
| Backend       | Node.js, Express                |
| Auth          | Firebase Authentication         |
| Database      | PostgreSQL (with PostGIS)       |
| Hosting       | Vercel (frontend), Render/Heroku (API) |
| Maps / Geo    | Mapbox API (or Google Maps)     |
| Email         | SendGrid / Nodemailer (MVP)     |

---

## 🗂 Project Structure

garagesalio-mvp/
├── api/           # Express backend
│   ├── index.js
│   └── ...routes
├── frontend/      # Next.js frontend
│   ├── pages/
│   ├── components/
│   └── ...
├── docker-compose.yml
├── README.md
└── .env.example


---

## ⚙️ Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/YOUR_USERNAME/garagesalio-mvp.git
cd garagesalio-mvp
````

### 2. Set up environment variables

Copy `.env.example` to both `/api/.env` and `/frontend/.env.local` and fill in the required values.

### 3. Start Postgres with Docker

```bash
docker-compose up
```

### 4. Start Backend API

```bash
cd api
npm install
npm run dev
```

Backend should now be running at: [http://localhost:4000](http://localhost:4000)

### 5. Start Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend should now be running at: [http://localhost:3000](http://localhost:3000)

---

## 🧪 API Example

```http
GET /api/ping

Response:
{
  "status": "OK",
  "time": "2025-06-19T15:45:12.123Z"
}
```

---

## 📦 Deployment

* **Frontend**: Deploy via [Vercel](https://vercel.com/)
* **Backend**: Deploy on [Render](https://render.com/) or [Heroku](https://heroku.com/)
* **Database**: Use AWS RDS, Supabase, or Neon for PostgreSQL in production

---

## 🛡 Security

* All API routes requiring authentication use Firebase ID tokens
* XSS & CSRF protection will be enforced through `next-auth` and secure HTTP-only cookies

---

## 💡 Roadmap

* [ ] Add boosted/sponsored listings
* [ ] Mobile PWA support
* [ ] SMS reminders
* [ ] Business/estate sale tier
* [ ] Analytics dashboard for sellers

---

## 🙌 Contributing

Pull requests welcome! To contribute:

1. Fork the project
2. Create a new branch (`git checkout -b feature/something`)
3. Commit your changes (`git commit -m 'Add something'`)
4. Push to the branch (`git push origin feature/something`)
5. Open a PR

---

## 📜 License

[MIT](LICENSE)

---

## 🔗 Links

* Project Site: *Coming soon*
* Figma Design: *Link here*
* GitHub Issues: [https://github.com/YOUR\_USERNAME/garagesalio-mvp/issues](https://github.com/YOUR_USERNAME/garagesalio-mvp/issues)

