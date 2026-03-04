# 🚀 Node.js Email Sending API (Plesk Ready)

Production-ready REST API for sending emails using SMTP.
Designed for deployment on **Plesk Node.js hosting**.

---

## ✨ Features

- ✅ Send emails via SMTP
- ✅ HTML email support
- ✅ API Key protection
- ✅ Rate limiting
- ✅ Environment-based configuration
- ✅ Production-ready for Plesk
- ✅ Compatible with Node.js 18+

---

## 🏗 Tech Stack

- Node.js
- Express
- Nodemailer
- dotenv
- express-rate-limit

---

## 📁 Project Structure


email-api/
│
├── index.js
├── .env
├── .env.example
├── package.json
└── README.md


---

## ⚙️ Installation

### 1️⃣ Clone repository

```bash
git clone https://github.com/yourusername/email-api.git
cd email-api
2️⃣ Install dependencies
npm install
🔐 Environment Variables

Create .env file:

PORT=3000

SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your_email@gmail.com
SMTP_PASS=your_app_password
SMTP_SECURE=false

API_KEY=supersecretkey

⚠️ Never commit .env to Git.

▶️ Run Locally
npm start

Server will run at:

http://localhost:3000
📤 API Usage
Endpoint
POST /api/send-email
Headers
Content-Type: application/json
x-api-key: your_api_key
Request Body
{
  "to": "client@email.com",
  "subject": "Test Email",
  "html": "<h1>Hello World 🚀</h1>"
}
Success Response
{
  "success": true,
  "messageId": "<message-id>"
}
🌐 Deploy on Plesk

Upload project to:

/var/www/vhosts/yourdomain.com/email-api/

Go to Plesk → Domains → Node.js

Set:

Application startup file: index.js

Application mode: production

Node version: 18+

Click:

NPM Install

Restart App

📦 Recommended SMTP Providers (Production)

Instead of Gmail, use professional email services:

SendGrid

Mailgun

Amazon SES

Better reliability, higher limits, fewer spam issues.

🛡 Production Security Tips

Use HTTPS only

Use strong API keys

Add rate limiting

Restrict server firewall rules

Use email service provider with domain verification (SPF, DKIM, DMARC)

🚀 Future Improvements (Optional)

Email queue (Redis)

Retry system

Logging system

Template engine (Handlebars)

TypeScript version

JWT authentication

Multi SMTP fallback

👨‍💻 Author

Your Name

📄 License

MIT
- 100k emails/day scalable architecture 🔥

Just tell me your goal 😎
