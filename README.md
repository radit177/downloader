# @r4ditt-sengkrep/downloader

Universal social media downloader — TikTok, Instagram, YouTube, Facebook

[![npm version](https://badge.fury.io/js/@r4ditt-sengkrep%2Fdownloader.svg)](https://badge.fury.io/js/@r4ditt-sengkrep%2Fdownloader)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-16%2B-green)](https://nodejs.org/)

---

## 📦 Installation

```bash
npm install @r4ditt-sengkrep/downloader
```

---

## 🚀 Usage

```javascript
import { tiktokDownloader, instagramDownloader, youtubeDownloader, facebookDownloader } from '@r4ditt-sengkrep/downloader';

// TikTok
const tiktok = await tiktokDownloader('https://vt.tiktok.com/xxxxx');

// Instagram
const ig = await instagramDownloader('https://www.instagram.com/p/xxxxx');

// YouTube (MP4)
const video = await youtubeDownloader('https://youtu.be/xxxxx', 'mp4');

// YouTube (MP3)
const audio = await youtubeDownloader('https://youtu.be/xxxxx', 'mp3');

// Facebook
const fb = await facebookDownloader('https://www.facebook.com/watch?v=xxxxx');
```

---

## 📊 Response

### Success

```json
{
  "success": true,
  "author": "r4ditt-sengkrep",
  "data": {
    "title": "Video Title",
    "download": "https://..."
  }
}
```

### Error

```json
{
  "success": false,
  "author": "r4ditt-sengkrep",
  "error": "Error message here"
}
```

---

## 🔧 Functions

| Function | Params | Returns |
|----------|--------|---------|
| `tiktokDownloader(url)` | TikTok URL | video HD/SD + audio + metadata |
| `instagramDownloader(url)` | Instagram URL | image/video download links |
| `youtubeDownloader(input, format)` | URL or keyword, 'mp4'/'mp3' | MP4 or MP3 download |
| `facebookDownloader(url)` | Facebook URL | video multiple quality |

---

## 📝 Changelog

**v1.0.1** (2026-07-25)
- Fixed Instagram regex
- Fixed YouTube search fallback
- Improved error handling

**v1.0.0** (2026-07-25)
- Initial release
- TikTok, Instagram, YouTube, Facebook support

---

## 👤 Author

**r4ditt-sengkrep (Radit DVC)**
- GitHub: [@radit177](https://github.com/radit177)
- Email: opditss@gmail.com
- npm: [@r4ditt-sengkrep](https://www.npmjs.com/~r4ditt-sengkrep)

---

## 📄 License

MIT — free to use, modify, and distribute

---

⭐ Star this repo if you find it useful!

*"I just give the tools, whether they're used right or not is your business, Boss."*
