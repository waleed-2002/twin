
Twin is a **full-stack application** with a **Python (FastAPI) backend** and a **Next.js (React + TypeScript) frontend**.

---

## 📁 Project Structure

```
twin/
├── backend/
│   ├── server.py
│   ├── requirements.txt
│   ├── pyproject.toml
│   └── me.txt
│
└── frontend/
    ├── app/
    ├── components/
    ├── public/
    ├── styles/
    ├── package.json
    ├── tsconfig.json
    └── ...
```

---

## 🚀 Backend

**Technology:** FastAPI (Python)
**Package Manager:** `uv`

### Prerequisite

Install `uv` (if not already installed):

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

---

### Install Dependencies

From the `backend/` directory:

```bash
uv pip install -r requirements.txt
```

> `uv` automatically manages a virtual environment.

---

### Run the Backend Server

```bash
uv run uvicorn server:app --reload
```

The backend will be available at:

```
http://localhost:8000
```

---

### Backend Configuration Files

* `server.py` — FastAPI application entry point
* `requirements.txt` — Python dependencies
* `pyproject.toml` — Build and project metadata

---

## 🎨 Frontend

**Technology:** Next.js (React + TypeScript)

### Install Dependencies

From the `frontend/` directory:

```bash
npm install
```

### Run the Development Server

```bash
npm run dev
```

The frontend will be available at:

```
http://localhost:3000
```

---

### Key Frontend Files

* `components/twin.tsx` — Main React component
* `app/page.tsx` — Home page
* `app/globals.css` — Global styles

---

## 🛠 Development Workflow

To run the full stack locally:

1. Start the backend using `uv`
2. Start the frontend dev server
3. Open `http://localhost:3000` in your browser

---

## 📝 Notes

* Ensure frontend API calls point to `http://localhost:8000`.
* Backend dependencies are managed using **`uv`** (`requirements.txt` / `pyproject.toml`).
* Frontend dependencies are managed using **npm** or **yarn**.

---

