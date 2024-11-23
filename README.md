**ke_sh : Bash Exercise Collection**  
Various shell scripts made for Linux.   
Tip: Add script folder to ENV in your .bashrc (or similar) and run the scripts anywhere! 

---

# kesplash

Bash Splash!
From neofetch to pfetch...to just a little bit more up-time stats:

![image](https://github.com/kedepot/ke_sh/assets/95410139/b1c657cf-aaad-427e-8c7b-f2b7d6283bcd)


### Info
- Uses 'last reboot' data to gather "approximate" data
- "Good enough" for my desktop use, as terminal splash screen trivia
- Only runs when called. (when I launch a Terminal window. No daemons or anything.)
- Customize directly in the script. 
- Made for Arch Linux
- Will need 'day' & 'day-se' too (just comment out that part if you prefer less text)

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
  
![image](https://github.com/kedepot/ke_sh/assets/95410139/ff0c793b-52f3-40db-bd22-1bcf008924c4)


**Format:** datecount 1989-10-03 2023-10-03  
(FROM-DATE TO-DATE using Year-Month-Day. Not tested with non-ISO8601 locales - may or may not work on those.)  

- Hyphens are not required
- If only a single date is provided, **today** is used as TO-DATE
- Only using the last 2 digits of a year will be counted as 1900's
- Try your birthdate (and despair)

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

# day
International UN days. 
- Some days may be moving dates (baded on UN2024 dates - close enough! (too much hassle to track!) 
- Use as-is (or as variable for other programs, like your terminal splash!)

---

# day-se
Similar to 'day' but only (mostly) Swedish theme-days (No holidays or moving dates though, again.) 
- Use as-is (or as variable for other programs, like your terminal splash!)

---
