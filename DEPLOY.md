# Deploy to Render

1. Push this project to GitHub.
2. In Render, create a Blueprint from the repository.
3. Render reads `render.yaml`.
4. Backend: set `JWT_SECRET` and `FRONTEND_URL`.
5. After backend deployment, set frontend `VITE_API_BASE_URL` to:
   `https://YOUR-BACKEND.onrender.com/api`
6. Set backend `FRONTEND_URL` to your frontend URL.

Important: the current backend uses in-memory demo data. It is not persistent yet.
For real production use, add a persistent database and object/file storage.
