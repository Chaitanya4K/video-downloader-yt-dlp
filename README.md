# video-downloader-yt-dlp
Complete guide to download YouTube videos using yt-dlp and FFmpeg on Windows.
# 🎬 YouTube Video Downloader using yt-dlp

![GitHub Repo stars](https://img.shields.io/github/stars/Chaitanya4K/youtube-video-downloader-yt-dlp?style=social)
![GitHub forks](https://img.shields.io/github/forks/Chaitanya4K/youtube-video-downloader-yt-dlp?style=social)
![License](https://img.shields.io/badge/license-MIT-blue)

A complete guide to downloading YouTube videos using **yt-dlp** and **FFmpeg** on Windows using Command Prompt.

This project explains how to:

✔ Download YouTube videos  
✔ Select video quality (720p / 1080p)  
✔ Merge video and audio streams  
✔ Download entire playlists  

---

# 📌 Technologies Used

- yt-dlp
- FFmpeg
- Windows Command Prompt
- GitHub

---

# 📥 1. Download yt-dlp

Download from:

https://github.com/yt-dlp/yt-dlp/releases

Download the file:

yt-dlp.exe

Create a folder on your system:

C:\yt-dlp video downloader


Move the file inside that folder.

Final folder structure:
C:
└── yt-dlp video downloader
└── yt-dlp.exe

---

# 🎞 2. Install FFmpeg

Download FFmpeg from:

https://www.gyan.dev/ffmpeg/builds/

Download:

ffmpeg-release-essentials.zip

Extract and move to:

C:\ffmpeg


Extract the folder and move it to:

C:\ffmpeg\bin\ffmpeg.exe

Final folder structure:
C:\ffmpeg
└── bin
├── ffmpeg.exe
├── ffplay.exe
└── ffprobe.exe

---

# 🔎 3. Verify FFmpeg Installation

Open Command Prompt and Run: 

C:\ffmpeg\bin\ffmpeg -version



If installed correctly you will see the FFmpeg version details.

---

# 📺 Step 4: Download a YouTube Video

Basic command:

yt-dlp VIDEO_URL

Example: yt-dlp https://www.youtube.com


This downloads the best available format.

---

# 📊 Step 5: Check Available Video Formats

yt-dlp -F VIDEO_URL

Example output:

36 mp4 720p
137 mp4 1080p
140 m4a audio

---

# 🎥 6. Download Specific Resolution

Example: Download **720p video**

yt-dlp -f 136+140 VIDEO_URL


Explanation:

| Format | Description |
|------|-------------|
| 136 | 720p video |
| 140 | audio |

---

# 🔧 Step 7: Merge Video and Audio using FFmpeg

yt-dlp --ffmpeg-location "C:\ffmpeg\bin" -f 136+140 VIDEO_URL


Process:

1. Download video stream  
2. Download audio stream  
3. Merge both using FFmpeg  
4. Create final video file  

---

# ⭐ 8 Download Best Quality Automatically

Recommended command:

yt-dlp --ffmpeg-location "C:\ffmpeg\bin" -f "bestvideo+bestaudio/best" VIDEO_URL


---

# 📥 9. Download Entire Playlist

yt-dlp PLAYLIST_URL

Example:

yt-dlp https://www.youtube.com/playlist?list=PLAYLIST_ID


Videos will download sequentially.

---

# 📂 10  Output Location

Downloaded videos are saved in the folder where the command is executed.

Example:

C:\yt-dlp video downloader


---

# ⚠ Common Errors

### Requested format is not available

Run: yt-dlp -F VIDEO_URL

Then select an available format.

---

### FFmpeg not installed

Add FFmpeg location:
--ffmpeg-location "C:\ffmpeg\bin"

----

# 👨‍💻 Author

**Chaitanya K**

Java Developer  
Spring Boot | Microservices | Kafka | REST APIs

---

# ⭐ Support

If you found this project helpful, please give it a **star** on GitHub.









