### **ke_sh : KE Bash Exercise Collection**  
Various shell scripts made for Linux.   
Tip: Add script folder to ENV in your .bashrc (or similar) and run the scripts anywhere! 
<br/>
<br/>

## kesplash

Bash Splash!
From neofetch to pfetch...to just a little bit more up-time stats:

![image](https://github.com/kedepot/ke_sh/assets/95410139/b1c657cf-aaad-427e-8c7b-f2b7d6283bcd)

### Info
- Uses 'last reboot' data to gather "approximate" data
- "Good enough" for my desktop use, as terminal splash screen trivia
- Only runs when called. (when I launch a Terminal window. No daemons or anything.)
- Customize directly in the script. 
- Made for Arch Linux
- Uses 'day' & 'day-se' by default, unless optional argument is passed (see below)

### Use
Run kesplash from the top of your .bashrc (or similar).  
or, Use/Modify as you see fit.

Optional Arguments:  
**nod** (no 'day'+'day-se') or  
**do** ('day' only) or  
**seo** ('day-se' only))  
ex: _kesplash nod_ (for no 'day' / 'day-se') - if you also have those scripts (from this depot)

NOTE: If you (or your distro) has /etc/logrotate.conf or something that clear your logs regularly, 
kesplash probably won't be useful.  
( For more advanced up-time statistics, check out:
https://github.com/rfmoz/tuptime )

<br/>

## datecount
Calculate days + other units of time between input dates
  
![image](https://github.com/kedepot/ke_sh/assets/95410139/ff0c793b-52f3-40db-bd22-1bcf008924c4)


**Format:** datecount 1989-10-03 2023-10-03  
FROM-DATE TO-DATE using Year-Month-Day.  
_Not tested with non-ISO8601 locales - may or may not work_

- Hyphens are not required
- If only a single date is provided, **today** is used as TO-DATE
- Only using the last 2 year-digits = "closest guess" for either 1900s or 2000s (by date cmd)
- Try your birthdate (and despair)

<br/>

## ketz
List Time Zones, in Shell script.

![image](https://user-images.githubusercontent.com/95410139/232210713-53559e23-61e3-47da-ac0e-25dfbe11f2bf.png)

Note: Easy enough to change both colors & locations, should you disagree with the choices!

<br/>

## zipseparate
Zip each selected folder or file separately
- Using [zip](https://man.archlinux.org/man/zip.1.en)
- When used for Custom Action for Thunar : Use %N (or %F)

<br/>

## mp423
Convert MP4 Audio to MP3

Usage example:  mp423 *.mp4  (converts all mp4s audio streams to new mp3 files)
- optional flag: -v converts MP3 to "visualized mp4"
- When used for Custom Action for Thunar : Use %N
- Has notifications for file(s) progress when used in Thunar (or other app - not terminal)
- Requires [ffmpeg](https://wiki.archlinux.org/title/FFmpeg)

<br/>

## day
International UN days.  

![2024-11-24_11-33](https://github.com/user-attachments/assets/d523c4ab-c96e-4d99-abbe-a22ada7ca8db)

- Some days may be moving dates (based on UN2024 dates - close enough! (too much hassle to track?) 
- Use as-is (or as variable for other programs, like your terminal splash!)
- No webscraping - just a big associative array.
- To-do: Support moving dates (maybe if I am real bored some day...)

<br/>

## day-se
Similar to 'day' but only (mostly) Swedish theme-days. In swedish!
- Use as-is (or as variable for other programs, like your terminal splash!)
- "Mostly", as some "special interest" (and joke-y) days are also included
- Does not include UN days or days with moving dates
- No religious holidays: a lot of them are moving dates (weird to just include "some" of these imho)

<br/>

## antiscrape  

![2024-11-25_10-09](https://github.com/user-attachments/assets/f7bb5bc5-61a6-43d1-aa2d-6ee8b83151e5)

Converts input text to html-code mixed with regular characters and commentes  
- Should work reasonably well against the dumbest scrapers
- No other conversions/efforts are needed, just paste into html document
- There are many online tools for this, but they come and go...
- Remember to quote the input if there are spaces!
