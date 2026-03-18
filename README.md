# 🎬 YouTube Clipper Tool

A simple yet powerful tool to clip videos directly from YouTube.

This project is designed as a scalable foundation for building a smart video clipping system, with future support for automation workflows and AI-assisted features.

---

## 🚀 Features

### ✅ Current Features

- Input YouTube URL
- Download video using `yt-dlp`
- Clip video using timestamp (start & end)
- Export clipped video

---

### 🔮 Coming Soon

- Multiple clip generation
- Smart clip suggestions (semi-automatic)
- Subtitle editor
- AI-powered highlight detection
- Workflow automation with n8n
- Batch processing

---

## 🧱 Project Structure

```
youtube-clipper-tool/
│
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── routes/
│   │   ├── services/
│   │   └── utils/
│   │
│   └── requirements.txt
│
├── frontend/        # Future UI (Web / Desktop)
├── n8n/             # Workflow automation (future)
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## ⚙️ Tech Stack

### Backend

- FastAPI
- yt-dlp
- ffmpeg

### Automation (Planned)

- n8n

### Future AI Integration

- Speech-to-text (Whisper)
- NLP for highlight detection

---

## 🧭 How It Works

### Basic Flow

1. User inputs a YouTube link
2. Backend downloads the video
3. User selects start & end timestamps
4. System clips the video using ffmpeg
5. Output video is ready to download

---

### Future Flow (With Automation & AI)

1. User inputs a YouTube link
2. Workflow (n8n) processes the video
3. System generates suggested clips
4. User selects preferred clip
5. Subtitle editing (optional)
6. Final export

---

## 🛠 Setup (Backend)

### 1. Clone Repository

```bash
git clone https://github.com/systemzerodev/youtube-clipper-tool.git
cd youtube-clipper-tool
```

---

### 2. Install Dependencies

```bash
cd backend
pip install -r requirements.txt
```

---

### 3. Install ffmpeg

Make sure ffmpeg is installed and accessible:

```bash
ffmpeg -version
```

---

### 4. Run Server

```bash
uvicorn app.main:app --reload
```

---

### 5. Open API Docs

```
http://127.0.0.1:8000/docs
```

---

## 🔌 API Endpoints (Basic)

### POST `/clip`

Clip a video from YouTube

**Params:**

- `url` → YouTube video link
- `start` → start timestamp (e.g. 00:01:00)
- `end` → end timestamp (e.g. 00:02:00)

---

## 🧠 Project Vision

This project starts as a simple clipping tool but is designed to evolve into a:

> 🎯 Smart Content Clipping System

Future possibilities:

- Auto-generate viral clips
- Content repurposing (TikTok / Shorts)
- AI-assisted editing pipeline
- Fully automated workflows

---

## ⚠️ Disclaimer

This project is intended for educational and personal use.

Please respect YouTube’s Terms of Service when downloading and using content.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

Built with ❤️ as part of a learning and experimentation journey in fullstack development, automation, and AI systems.
