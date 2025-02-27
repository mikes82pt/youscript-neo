========================================================== ===================
YOUSCRIPT-NEO
========================================================== ===================

Manual: v0.53

It is recommended to consult the URL https://bytes.lunanet.ovh/youscript/readme.html
for a possible more up-to-date version of this manual.


- What is it

- Installation

- How to use

- License


-------------------------------------------------- -------------------
What is it
-------------------------------------------------- -------------------

It is a public domain video downloader.

Main capabilities:

- Download videos from any website.
- Browses the site and download the videos it finds.
- Download multiple videos according to the list of URLs.
- Resume the download(s) if the internet connection is lost.


-------------------------------------------------- -------------------
Installation
-------------------------------------------------- -------------------

Navigate to the website: https://bytes.lunanet.ovh/youscript/

Download the latest version suitable for your system.

Note: Youtube-DL requires Microsoft Visual C++ 2010 Redistributable Package (x86)
Available from: https://download.microsoft.com/download/1/6/5/165255E7-1014-4D0A-B094-B6A430A6BFFC/vcredist_x86.exe

Once downloaded, unzip the file to a folder of your choice.

The folder "youscript-neo" will be created with the following folders:

- bin
- scripts
- videos (this is where the videos will be downloaded)

In the "youscript-neo" folder you will also find the files:

- menu.bat (the main menu)
- url.txt (automatically created by menu.bat if not found)


-------------------------------------------------- -------------------
How to use
-------------------------------------------------- -------------------

Interaction with YOUSCRIPT-NEO is essentially done through the
main menu:

1) In the file explorer, double click on the file: menu.bat

2) Or, using the command line:

- Open a shell (cmd, powershell, ...)
- Navigate to the YOUSCRIPT-NEO installation folder
- Run the file: menu.bat


YOUSCRIPT-NEO will try to download the videos indicated in the url.txt file.

Write in that file one URL per line.
Note: Lines beginning with # are ignored.
The url.txt file can be opened in the menu using the "a" option

----------------------------
Main menu options:
----------------------------


- 1 Default

Download the videos indicated in the url.txt file.
Download in the best possible quality and in the best possible codec,
not necessarily what the user might want.

- 2 Up to 1080p H264
- 3 Up to 720p H264
- 4 Up to 480p H264
- 5 Up to 360p H264

Instead of using the best quality (and codec) available, use the one indicated
(or lower, if the indicated box does not exist).

- 6 Youtube audio only

In the case of YouTube videos, download only the audio.

- 7 List formats

For each given URL, list the formats that are available
for download.

- 8 Organize files

Move downloaded files from ./videos to ./videos/yt

Note: "yt" in case of YouTube videos.
The program tries to organize the videos by folders as best it can.

- 9 Update

Update or update yt-dlp, the YOUSCRIPT-NEO engine (the scripts
are not updated). It is essential to update if YOUSCRIPT-NEO
unable to download from any particular site.

- a Open url list file

Open the url.txt file with notepad.
Then just enter the URL's here. (1 URL per line)


- x Extra

Extra options: for those who know what they are doing. who needs
reading the manual should not use these options.

- r Clean url.txt

Remove the contents of the url.txt file (the file itself is not deleted).

- h Help

Open notepad with this file.

- 0 exit

Leave the menu. Exit YOUSCRIPT-NEO. Return to explorer (or shell).


-------------------------------------------------- -------------------
License
-------------------------------------------------- -------------------

Public domain.

Unlicence: https://unlicense.org/




-------------------------------------------------- -------------------
What's new?
-------------------------------------------------- -------------------
Version 0.53 2023-07-09
-Update of ffmpeg from version 5.1.2 to version 6.0 (64bit only)
-Small correction in the extra menu


Version 0.52 2023-02-04
-Small resolution to solve the problem of file organization not always working;
-Update of ffmpeg from version 5.1 to version 5.1.2 (64bit only)
-Small correction in the extra menu


Version 0.51 01-30-2023
-The "8 Organize files" option now organizes based on information in the metadata instead of the file name;
-Small optimizations in folder management and bug fixing.



Version 0.50 2023-01-22
- Menu "ask for url" was removed and replaced by the option to open url.txt file in the menu;
- Videos are transferred with the metadata
