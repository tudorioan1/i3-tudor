# i3-tudor
#### Note : This might need additional troubleshooting.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b1bb752f-12ba-4bb1-8c92-d0b38c35cc83" />

1. Install the required dependencies : i3, picom, dunst, rofi, polybar, flameshot, thunar, alacritty, quickshell, xdotool, feh, JetBrainsMono Nerd Font, Material Icons + Feather fonts (bundled in `polybar-i3/fonts`).
2. Clone the repository anywhere (for example `~/i3-tudor`):

   ```bash
   git clone https://github.com/tudorioan1/i3-tudor ~/i3-tudor
   ```

3. Copy the configs into `~/.config`. Polybar **must** end up in `~/.config/i3/polybar-i3` (every path in the polybar config points there):

   ```bash
   mkdir -p ~/.config/i3
   cp -r ~/i3-tudor/i3/. ~/.config/i3/
   cp -r ~/i3-tudor/polybar-i3 ~/.config/i3/polybar-i3
   cp -r ~/i3-tudor/{alacritty,dunst,picom,rofi,quickshell} ~/.config/
   chmod +x ~/.config/i3/polybar-i3/launch.sh ~/.config/i3/polybar-i3/scripts/*.sh \
            ~/.config/i3/polybar-i3/scripts/weather/weather.sh ~/.config/i3/lock \
            ~/.config/rofi/powermenu.sh ~/.config/quickshell/wallpaper-picker/toggle.sh
   ```

4. Test the bar manually (errors are printed in the terminal):

   ```bash
   ~/.config/i3/polybar-i3/launch.sh
   ```

Launch i3 from your display manager (SDDM, GDM, LightDM, Ly etc.) and enjoy.
