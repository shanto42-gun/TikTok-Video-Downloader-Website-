<img width="1917" height="827" alt="image" src="https://github.com/user-attachments/assets/dab14a54-15d4-425e-ba90-ded460add907" /><img width="1917" height="827" alt="image" src="https://github.com/user-attachments/assets/2391e93b-184c-493a-9bba-96acfb2932ee" />
# TikSave — Modern TikTok Video, Story & Audio Downloader
See my Website Live : https://tiktokvidoedownloder-shanto.netlify.app/
> Premium, fast, watermark-free TikTok media downloader built with Next.js 14, TypeScript, and Tailwind CSS.

## 🚀 Features

- **No Watermark Video Downloads**: Clean HD 1080p MP4 downloads directly to phone or PC.
- **24h Story Saver**: Download TikTok stories before they disappear.
- **Photo Slideshows**: Full preview of multi-photo posts with individual JPG or bulk ZIP downloads.
- **MP3 Audio Extraction**: Extract trending audio tracks and sounds in 320kbps MP3 format.
- **Clipboard Auto-Paste**: Instant paste detection with single-click workflow.
- **Dynamic Loading States**: Shimmer skeleton cards and cycling micro-copy feedback.
- **Security & Privacy**: Strict domain allowlists, SSRF prevention, sliding-window rate limiting, and zero file retention.
- **Mobile First & Responsive**: Optimized for iOS Safari, Android Chrome, and desktop screens.
- **Full SEO Optimization**: Semantic HTML5, dynamic Open Graph tags, sitemap.xml, and robots.txt.

## 🛠️ Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS + Custom Glassmorphism UI
- **Icons**: Lucide React
- **API**: Next.js Node.js Edge/Route Handlers

## 📦 Getting Started

### 1. Install dependencies
```bash
npm install
```

### 2. Run the development server
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### 3. Production Build
```bash
npm run build
npm run start
```

## 🌐 API Contract

### `POST /api/download`
**Request Payload:**
```json
{
  "url": "https://www.tiktok.com/@user/video/7192849182749102382",
  "type": "video"
}
```

**Success Response (200 OK):**
```json
{
  "status": "success",
  "type": "video",
  "id": "video_123456",
  "creator": {
    "username": "@creator",
    "nickname": "Creator",
    "avatar": "https://...",
    "verified": true
  },
  "caption": "Video description...",
  "thumbnail": "https://...",
  "duration": 38,
  "statistics": { "likes": "482K", "views": "2.4M" },
  "music": { "title": "Sound Title", "author": "Sound Artist" },
  "downloads": [
    { "label": "Download MP4 (No Watermark)", "url": "https://...", "format": "mp4", "quality": "1080p HD", "isHd": true },
    { "label": "Download Audio Only (MP3)", "url": "https://...", "format": "mp3", "quality": "320kbps" }
  ]
}
```

## ⚖️ Legal & DMCA Notice
TikSave does not host or store any media files on its servers. All media is fetched directly from TikTok's CDN. This application is not affiliated with, sponsored by, or endorsed by TikTok or ByteDance Ltd.
