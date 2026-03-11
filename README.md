# video-downloader-yt-dlp
Complete guide to download YouTube videos using yt-dlp and FFmpeg on Windows.
# YouTube Video Downloader using yt-dlp

This project explains how to download YouTube videos using **yt-dlp** and **FFmpeg** on Windows.

## Tools Used

- yt-dlp
- FFmpeg
- Windows Command Prompt

---

# 1. Download yt-dlp

Download from:

https://github.com/yt-dlp/yt-dlp/releases

Download the file:

yt-dlp.exe

Create a folder:

C:\yt-dlp video downloader

Move the file inside that folder.

---

# 2. Install FFmpeg

Download FFmpeg from:

https://www.gyan.dev/ffmpeg/builds/

Extract and move to:

C:\ffmpeg

Folder structure:

C:\ffmpeg\bin\ffmpeg.exe

---

# 3. Verify FFmpeg Installation

Run: 

C:\ffmpeg\bin\ffmpeg -version


If installed correctly you will see version details.

---

# 4. Download a Video

yt-dlp VIDEO_URL

Example: yt-dlp https://www.youtube.com


---

# 5. List Available Formats

yt-dlp -F VIDEO_URL

Example output:

36 mp4 720p
137 mp4 1080p
140 m4a audio


---

# 6. Download Specific Resolution

Example: 720p

yt-dlp -f 136+140 VIDEO_URL


---

# 7. Merge Video and Audio using FFmpeg

yt-dlp --ffmpeg-location "C:\ffmpeg\bin" -f 136+140 VIDEO_URL


---

# 8. Download Best Quality Automatically

yt-dlp --ffmpeg-location "C:\ffmpeg\bin" -f "bestvideo+bestaudio/best" VIDEO_URL


---

# 9. Download Entire Playlist

yt-dlp PLAYLIST_URL


---

# 10. Output Location

Videos are saved in the folder where the command is executed.

Example:

C:\yt-dlp video downloader

---

# Author

Chaitanya K  
Java Developer | Spring Boot | Microservices | Kafka










