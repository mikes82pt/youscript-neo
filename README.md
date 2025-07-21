YOUSCRIPT-NEO  


---

**Table of Contents**  
- What is it  
- Installation  
- How to use  
- License  

---

**What is it**  

YOUSCRIPT-NEO is a public domain video downloader.  

Main capabilities:
- Download videos from any website.
- Browse the site and download videos it finds.
- Download multiple videos based on a list of URLs.
- Resume downloads if the internet connection is lost.

---

**Installation**  

1. Navigate to the website:  
https://github.com/mikes82pt/youscript-neo

2. Download the latest version suitable for your system.

**Note**: YouTube-DL requires the Microsoft Visual C++ 2010 Redistributable Package (x86).  
Available for download at:  
https://download.microsoft.com/download/1/6/5/165255E7-1014-4D0A-B094-B6A430A6BFFC/vcredist_x86.exe

3. Once downloaded, unzip the file to a folder of your choice.

The folder "youscript-neo" will be created with the following subfolders:  
- bin  
- scripts  
- videos (where the videos will be downloaded)

The "youscript-neo" folder will also contain these files:  
- menu.bat (the main menu)  
- url.txt (automatically created by menu.bat if not found)

---

**How to Use**  

Interaction with YOUSCRIPT-NEO is mainly done through the main menu.

1. In the file explorer, double-click on the file: menu.bat.
2. Or, using the command line:
   - Open a shell (cmd, PowerShell, etc.)
   - Navigate to the YOUSCRIPT-NEO installation folder.
   - Run the file: menu.bat.

YOUSCRIPT-NEO will attempt to download the videos listed in the url.txt file.

- Write one URL per line in the url.txt file.  
- Lines beginning with "#" are ignored.  
- You can open the url.txt file from the menu using the "a" option.

---

**Main Menu Options:**

1) Default  
Download the videos listed in url.txt. Downloads will be in the best possible quality and codec, which may not necessarily be the user's preference.

2) Up to 1080p H264  
Download videos up to 1080p with the H264 codec.

3) Up to 720p H264  
Download videos up to 720p with the H264 codec.

4) Up to 480p H264  
Download videos up to 480p with the H264 codec.

5) Up to 360p H264  
Download videos up to 360p with the H264 codec.

6) YouTube Audio Only  
For YouTube videos, download only the audio.

7) List Formats  
For each given URL, list the formats available for download.

8) Organize Files  
Move downloaded files from ./videos to ./videos/yt.  
Note: "yt" for YouTube videos. The program will attempt to organize the videos into folders as best as it can.

9) Update  
Update yt-dlp, the YOUSCRIPT-NEO engine (scripts are not updated).  
It's important to update if YOUSCRIPT-NEO fails to download from a particular site.

a) Open URL List File  
Open url.txt in Notepad. You can then add URLs (one per line).

x) Extra  
Extra options for advanced users. If you're unsure, don't use these options.

r) Clean URL List  
Remove the contents of url.txt (the file itself is not deleted).

h) Help  
Open this file in Notepad.

q) Exit  
Exit the menu and return to the file explorer or shell.

---

**License**  

Public Domain  
Unlicense: https://unlicense.org/

---

**What's New?**

Version 0.55 (2025-07-20)

Downloads folder renamed from "Videos" to "Media."
- "Ignore Errors" feature removed.
- Added option to retrieve only filenames.
- FFmpeg version updated to 7.1.1.


Version 0.54 (2025-01-26)
- Updated FFmpeg from version 6.0 to 7.1 (64-bit only).
- A backup is created when url.txt is deleted.
- Menu changes: "q" is now used to exit, instead of "0" or nothing.
- Cleaned up old code.


Version 0.53 (2023-07-09)  
- Updated ffmpeg from version 5.1.2 to 6.0 (64bit only).  
- Small correction in the extra menu.

Version 0.52 (2023-02-04)  
- Fixed issue with file organization not always working.  
- Updated ffmpeg from version 5.1 to 5.1.2 (64bit only).  
- Small correction in the extra menu.

Version 0.51 (2023-01-30)  
- The "8 Organize Files" option now organizes based on metadata instead of file name.  
- Small optimizations in folder management and bug fixes.

Version 0.50 (2023-01-22)  
- Removed the "Ask for URL" menu and replaced it with the option to open url.txt.  
- Videos are now transferred with metadata.

---
