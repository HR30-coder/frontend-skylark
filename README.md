Project Title: RTSP Stream Manager - Frontend

Description:
-------------
This is the frontend of a full-stack RTSP Stream Viewer application built using React. It serves as a CRUD interface for managing RTSP stream links, communicates with a Django backend via REST APIs, and provides HLS-based video playback using `video.js`.

Key Features:
--------------
1. 📋 Create, edit, and view RTSP stream links.
2. 🎥 Stream viewer page using `video.js` for smooth HLS playback.
3. ⚠️ Error handling with user-friendly warning messages.
4. ⏯️ Playback begins automatically once HLS segments are detected.

Tech Stack:
------------
- React (with Hooks)
- Axios (for HTTP requests)
- React Router
- video.js
- JavaScript (ES6+)
- Vite (for fast bundling)

Local Setup Instructions:
---------------------------
1. Clone the repository:
   git clone <your_frontend_repo_url>

2. Navigate to the project folder:
   cd frontend

3. Install dependencies:
   npm install

4. Run the development server:
   npm run dev

   🔌 The frontend will be available at: http://localhost:5173

Environment Configuration:
---------------------------
- Ensure the backend is running on: http://127.0.0.1:8080
- You may create a `.env` file and set:
   VITE_API_BASE_URL=http://127.0.0.1:8080/api/

Folder Structure:
------------------
- /src
  ├── components/       # UI and form components
  ├── pages/            # Route-based pages
  ├── api/              # Axios service
  └── App.jsx           # Main entry point and routing

Notes:
-------
- Designed to work with the Django backend.
- Expects valid HLS (.m3u8) links from the server.
- Can be extended to support MJPEG streaming via WebSockets if needed.
