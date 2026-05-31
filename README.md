# ASAN VMS - Application System

A fully functional web application for managing citizen applications. Includes AI (Gemini)-powered automatic analysis, image upload, EXIF location extraction, and an admin verification system.

## Project Structure

```
aiasan/
├── backend/    # Node.js + Express + MongoDB API
├── admin/      # React (Vite) - Admin paneli
└── user/       # React (Vite) - Vətəndaş paneli
```

## Technologies

- **Backend:** Node.js, Express, MongoDB, Mongoose, Gemini AI
- **Frontend:** React, Vite, Tailwind CSS, Axios, Lucide Icons
- **Digər:** JWT Authentication, EXIF GPS extraction, Multer file upload

## Installation

### 1. Backend
```bash
cd backend
npm install
```

`.env` faylı yaradın:
```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
PORT=5000
```

```bash
node app.js
```

### 2. Admin Panel
```bash
cd admin
npm install
npm run dev
```

### 3. Citizen Dashboard
```bash
cd user
npm install
npm run dev
```

## Əsas Xüsusiyyətlər

- 📸 Image upload and camera capture
- 🤖 Automatic category, priority, and description generation using Gemini AI
- 📍 GPS extraction from EXIF metadata
- 👨‍💼 Admin panel for request management, editing, and verification
- ✅ Resolution verification system (AI-based comparison)
- ❌ Rejection system with reason tracking
- 🌐 Full Azerbaijani language support
