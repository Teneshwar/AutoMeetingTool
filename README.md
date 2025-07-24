# 🤖 Auto Meeting Tool

A powerful automation tool that automatically joins online meetings on **Google Meet**, **Microsoft Teams**, and **Zoom**, while providing **real-time transcription** and **speaker detection**.

---

## 🚀 Features

- ✅ **Auto-Join Meetings** – Automatically join scheduled meetings on Google Meet, Microsoft Teams, and Zoom using Puppeteer.
- 📝 **Real-Time Transcription** – Capture spoken content live during meetings using Google Speech-to-Text API.
- 🧠 **Speaker Detection** – Identify who is speaking during the call using smart voice segmentation.
- 💾 **Save to TXT File** – Export complete meeting transcripts into `.txt` files.
- 🔐 **Authentication** – Secure login & signup system using **JWT** and **JStAuth**.
- 📅 **Calendar Sync** – Syncs with calendar to auto-detect meeting times.
- ⚙️ **Tech Stack** – Built with modern technologies for seamless performance and scalability.

---

## 🛠️ Built With

### 💻 Frontend:
- [React.js](https://reactjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Vite](https://vitejs.dev/) 

### 🌐 Backend:
- [Node.js](https://nodejs.org/)
- [Express.js](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)

### 🧠 AI & Automation:
- [Puppeteer](https://pptr.dev/) – Browser automation
- [Google Speech-to-Text API](https://cloud.google.com/speech-to-text) – Real-time transcription
- Speaker Detection – Custom logic or available models for identifying speakers

### 🔐 Auth:
- JWT (JSON Web Token)
- JStAuth (for secure auth flows)

---

## 📂 Folder Structure

AutoMeetingTool/
│
├── client/ # Frontend (React + Tailwind + Vite)
│ ├── src/ # All React components and pages
│ ├── public/
│ ├── index.html
│ └── vite.config.js
│
├── server/ # Backend (Express + MongoDB + Puppeteer)
│ ├── config/ # MongoDB & other configs
│ ├── controllers/ # Route controllers
│ ├── routes/ # Express routes
│ ├── models/ # Mongoose models
│ ├── services/ # Puppeteer + transcription logic
│ ├── meeting-automator/ # Automation logic (auto-join)
│ ├── transcriptions/ # Stores generated .txt files
│ ├── debug_screenshots/ # Screenshots from Puppeteer for debugging
│ ├── server.js # Main backend entry point
│ └── .env # Environment variables

## ⚙️ Installation & Setup

### 1. Clone the Repository

git clone https://github.com/Teneshwar/AutoMeetingTool.git
cd AutoMeetingTool


### 2. Set Up Backend
cd server
npm install
Create a .env file in /server:
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GOOGLE_API_KEY=your_google_speech_to_text_api_key

Start the backend:
node server.js

### 3. Set Up Frontend
cd ../client
npm install
npm run dev
