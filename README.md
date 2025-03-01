<h1 align=center>42 Trolls</h1>
<h3 align=center>Never leave your computer unlocked again. 😈</h3>

Welcome to **42 Trolls** ! Here's the best command to prank your friends at 42 school.

We have sort them into 4 categories.
- **🟢 Slightly Annoying :** Simple prank which can easily be undone (like modify the .zshrc)
- **🟡 Moderately Annoying :** More ? This is the more accurate section ! Here some command that can be removed, but you have to know the tips. 😘
- **🟠 Very Annoying :** You like it ? Now take some hardware capabilities... Like sound, graphics, and why not some storage ?
- **🔴 Ultra Annoying :** The final (countdown ?)... Ultra annoying section, like session script or reset.

## 🟢 Slightly Annoying
Simple prank which can easily be undone (like modify the .zshrc)

### Lock your friend's screen  
Simply lock the screen of your current mate.
```bash
ft_lock
```

### 🎬 Lowcost Matrix
You always want to be an actor of the Matrix movies ? Create a Matrix effect, but without the money needed to pay for developers. 
```bash
echo 'cat /dev/urandom' >> ~/.zshrc
```
<details>
  <summary>🧹 How to remove ?</summary>

Use this command :
```bash
sed -i '' "s/cat \/dev\/urandom//g" ~/.zshrc
```
Or remove the line at end of the `.zshrc` file.
</details>

### 🐱 Tac or cat ?
Replace the cat command by rev, which is printing the file but reversed.
```bash
echo 'alias cat="rev"' >> ~/.zshrc
```
<details>
  <summary>🧹 How to remove ?</summary>

Use this command :
```bash
sed -i '' "s/alias cat=\"rev\"//g" ~/.zshrc
```
Or remove the line at end of the `.zshrc` file.
</details>

### 📖 Where is the fucking manual ?
Replace the man command by printing `No manual entry for {command}`. Pretty funny. 
```bash
echo 'man() { echo "No manual entry for $1"; }' >> ~/.zshrc
```
<details>
  <summary>🧹 How to remove ?</summary>

Use this command :
```bash
sed -i '' "s/man() { echo \"No manual entry for $1\"; }//g" ~/.zshrc
```
Or remove the line at end of the `.zshrc` file.
</details>

## 🟡 Moderately Annoying  
Some command that can be removed, but you have to know the tips. 😘

### 📺 AdSh - Ads in your shell
Worries about the free and no distrubtive shell ? Don't worries, you can now add ads when you type command on your terminal.

```bash
curl https://raw.githubusercontent.com/godetremy/42-trolls/refs/heads/main/adsh/install.sh | bash
```

<details>
  <summary>🧹 How to remove ?</summary>

Use this command :
```bash
curl https://raw.githubusercontent.com/godetremy/42-trolls/refs/heads/main/adsh/uninstall.sh | bash
```
Or remove the line at end of the `.zshrc` file, then delete the folder `.adsh` in your home.
</details>

<details>
  <summary>🪄 Want to contribute ?</summary>

You can add your own add in `adsh/video`, but don't forget :
- **2mb max video size :** This will impact the download speed. Much faster = much easier to prank. 👽
- **No 4K video :** Too big resolution will create lags in `mpv`, plus this is not important, terminal will not load a video in 1920x1080.

Now your video is added, don't forget to add it in the video variable, in `adsh/install.sh` and `adsh/adsh.sh`
</details>

## 🟠 Very Annoying  
Take some hardware capabilities... Like sound, graphics, and why not some storage ?

### 🕺 Rickrolled
Set the volume at 75%, and play _Never Gonna Give You Up_ by _Rick Astley_ in VLC fullscreen.
```bash
pactl set-sink-mute @DEFAULT_SINK@ false && pactl set-sink-volume @DEFAULT_SINK@ 75% && vlc https://dn720407.ca.archive.org/0/items/rick-roll/Rick%20Roll.ia.mp4 -f --no-video-title-show --mouse-hide-timeout 0
```

## 🔴 Ultra Annoying  
Ultra annoying section, like session script or reset. Only use if your friend is actually your **enemy**. 😈

### 💾 420T
Because 5Go is too small, live the expreience of the session of 420T.
```bash
echo '/usr/bin/zenity --error --title="bocal" --text="Your home is full! (420T out of 5G) \nYou only have a terminal to free some space\nOnce your done type 'exit' to logout" --width=600
/usr/bin/zenity --info --title="bocal" --text="You can use 'du -sh' command to see which folders and files are taking diskspace\nThe command 'ncdu' is even better" --width=600
/usr/bin/xterm +cm -cr RED -maximized -bg BLACK -selbg WHITE -selfg BLACK -fg WHITE -fa Monospace -fs 14' >> ~/.profile
```

### 🗑️ Files ? Which files ?
Some file to clear ? Why not all ? This will reset the session.
> [!CAUTION]
> This action cannot be undone. This more than a troll here. All his session will be removed. Be sure to have the approval of your friends.
```bash
touch ~/.reset
```
