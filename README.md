## tomato 

Simple Pomodoro timer for Linux implemented as a single Bash script.  

Displays a simple desktop notification and plays a sound (default damn-son.mp3) after the end of each Pomodoro.

---

### Dependencies

All dependencies available on official Arch repository and can be installed using 'pacman -S &lt;package-name&gt;'

 - **libnotify**
 - **pulseaudio-utils**

---

### Instructions 

**Arch Linux**

1. `$ git clone https://github.com/tony-redekop/tomato.git`
2. `$ cd tomato`
3. `$ cp tomato damn-son.mp3 /usr/local/bin`
4. `$ sudo chmod +x tomato damn-son.mp3`

---

### Usage

Usage: `tomato [-p POMODORO] [-s BREAK_TIME] [-n NUM_POMODOROS]`

  -p: Pomodoro length (in minutes), default: $POMODORO_TIME

  -s: Break length (in minutes), default: $BREAK_TIME

  -n: Number of Pomodoro cycles, default: $NUM_POMODOROS

---

### Customization

  Refactor the `notify-complete` function within the script to customize the alert sound and the displayed icon.