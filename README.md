**ke_sh : Bash Exercise Collection**  
Various shell scripts made for Linux.   
Tip: Add script folder to ENV in your .bashrc (or similar) and run the scripts anywhere! 

---

# kesplash

Bash Splash!
From neofetch to pfetch...to just a little bit more up-time stats:

![kesplashimg](https://github.com/kedepot/kesplash/assets/95410139/581958df-6e11-4fb1-978f-47f82443cc93)

### Info
- Uses 'last reboot' data to gather "approximate" data
- "Good enough" for my desktop use, as terminal splash screen trivia
- Only runs when called. (when I launch a Terminal window. No daemons or anything.)
- Customize directly in the script. 
- Compatible with most shells & distros. Probably. (not POSIX)

### Use
Run kesplash from the top of your .bashrc (or similar).  
Feel free to tweak the colours and formatting to whatever you prefer!

NOTE: If you (or your distro) has /etc/logrotate.conf or something that clear your logs regularly, 
kesplash probably won't be useful.  
( For more advanced up-time statistics, check out:
https://github.com/rfmoz/tuptime )

---

# datecount
Calculate days + other units of time between input dates
  
![datecount](https://github.com/kedepot/datecount/assets/95410139/baa683f5-ad32-4696-9de7-86d040a1b619)

**Format:** datecount 1989-10-03 2023-10-03  
(FROM-DATE TO-DATE using Year-Month-Day. Not tested with non-ISO8601 locales - may or may not work on those.)  

- Hyphens are not required
- If only a single date is provided, **today** is used as TO-DATE
- Only using the last 2 digits of a year will be counted as 1900's

---

# ketz
List Time Zones, in Shell script.

![image](https://user-images.githubusercontent.com/95410139/232210713-53559e23-61e3-47da-ac0e-25dfbe11f2bf.png)

Note: Easy enough to change both colors & locations, should you disagree with the choices!

---

# zipseparate
Zip each selected folder or file separately
- Using [zip](https://man.archlinux.org/man/zip.1.en)
- When used for Custom Action for Thunar : Use %N (or %F)

---

# mp423
Convert MP4 Audio to MP3

Usage example:  mp423 *.mp4  (converts all mp4s audio streams to new mp3 files)
- optional flag: -v converts MP3 to "visualized mp4"
- When used for Custom Action for Thunar : Use %N
- Has notifications for file(s) progress when used in Thunar (or other app - not terminal)
- Requires [ffmpeg](https://wiki.archlinux.org/title/FFmpeg)

---


