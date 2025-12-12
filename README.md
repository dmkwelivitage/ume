# 🚀 Profiles Module Setup & Testing Guide

Hey team! Here's a casual guide to get your **frontend and backend for Profiles** up and running 😎

## 1. Fetch the Code 📝

switch to the dev branch:

```bash

git checkout dev

```
---

## 2. Backend Setup ⚙️

1. Go to the backend folder:
```bash
cd backend
```
2. Install dependencies:
```bash
npm i
```
3. Add CORS so the frontend can talk to it:

- Import cors: `import cors from "cors";`
- Add middleware: `app.use(cors());`

Now your backend is ready to accept requests from the frontend 🌐

---

## 3. Frontend Setup 💻

1. Navigate to the frontend folder:
```bash
cd frontend
```
2. Install dependencies:
```bash
npm i
```
3. Create a `.env` file in the root and add your backend URL:

VITE_API_BASE_URL=[http://localhost:5000/api](http://localhost:5000/api)

This lets the frontend communicate with the backend. Easy peasy ✨

---

## 4. Frontend Folder Structure & Files 📁

### 4.1 api/
- **axios.ts**: Axios instance with base URL & credentials for all API calls.
- **endpoints.ts**: All API endpoints neatly organized (auth, user, profiles).

### 4.2 services/
- **profileService.ts**: Handles **CRUD operations** for profiles.

### 4.3 types/
- **profile.ts**: Type definitions for profile objects returned from the backend.

### 4.4 hooks/
- **useProfiles.ts**: Custom hook to fetch profiles and manage state (loading, data).

### 4.5 components/
- **ProfileCard.tsx**: Shows each profile in a card format.
- **Navbar.tsx**: Navigation bar.

### 4.6 pages/
- **Login.tsx**: Login page.
- **Dashboard.tsx**: Dashboard page.
- **Profiles.tsx**: Shows all profiles using `useProfiles` hook.

### 4.7 tests/
- **TestProfileCRUD.tsx**: Super handy test page to check **full CRUD flow**! Create, update, delete, refresh — everything is logged in the console and displayed on screen 🧪

---

## 5. Running the App ▶️

### Backend:
```bash
cd backend
npm run dev
```
### Frontend:
```bash
cd frontend
npm run dev
```
### Test CRUD:
Open your browser at: [http://localhost:5173/test-profile-crud](http://localhost:5173/test-profile-crud)

You should see all profiles from the backend and can test create, update, delete, and refresh 💡

---

## 6. Quick Recap ✅

- Fetched code & switched to `dev` branch.
- Backend: installed dependencies + added CORS.
- Frontend: installed dependencies, created `.env`, and added backend URL.
- Frontend is organized into **api, services, types, hooks, components, pages, tests**.
- `TestProfileCRUD.tsx` lets you verify the **full CRUD flow**.
- Everything is **modular, scalable, and ready for testing and development** 🎉

---

## 7. Additional Resources 📚

Read This Before You Start Working: [Read This Please](./UMESEYESONLY.md)  
*Make sure you are alone when reading 😉*

