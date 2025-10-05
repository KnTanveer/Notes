
### 1. Download yt-dlp
- Get the latest Windows .exe from:  
  👉 https://github.com/yt-dlp/yt-dlp/releases
- Place `yt-dlp.exe` somewhere easy, like:

C:\yt-dlp\

---

### 2. Install FFmpeg

#### A. Download:
- Go to: 👉 https://www.gyan.dev/ffmpeg/builds/
- Download: `ffmpeg-release-essentials.zip`
- Extract the contents (you’ll get a folder like `ffmpeg-6.x.x-essentials_build`)

#### B. Move to:

C:\ffmpeg\


You should now have:


C:\ffmpeg\bin\ffmpeg.exe  
C:\ffmpeg\bin\ffprobe.exe

#### C. Add FFmpeg to PATH:
1. Search: **Edit environment variables**
2. Under **System variables** → find `Path` → click **Edit**
3. Click **New**, add:

C:\ffmpeg\bin

4. Click OK on all dialogs
5. **Restart Command Prompt**

---

### Usage Example

1. Open Command Prompt
2. Navigate to yt-dlp folder:

cd C:\yt-dlp

3. Run download command:

`yt-dlp -x --audio-format mp3 "https://www.youtube.com/playlist?list=YOUR_PLAYLIST_ID"`

Replace the link with your actual YouTube playlist URL.

---

### Optional: Without adding FFmpeg to PATH

If you don’t want to edit system variables:

`yt-dlp.exe -x --audio-format mp3 "https://www.youtube.com/playlist?list=YOUR_PLAYLIST_ID" --ffmpeg-location "C:\ffmpeg\bin"`

### Output

- MP3 files will be saved in the same directory where you ran the command.
- Filenames include video titles automatically.

---

### Notes

- Only use for personal content or content you have rights to download.
- You can also download individual videos the same way.
