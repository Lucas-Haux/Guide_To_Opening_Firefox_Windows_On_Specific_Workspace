# Guide_To_Opening_Firefox_Windows_On_Specific_Workspace
Guide and script for automatically opening Firefox windows on specific workspaces in Hyprland. While designed with Hyprland in mind, the general concept can be adapted for other window managers with similar functionality.

## Requirements 
- [Window Titler Extension](https://github.com/tpamula/webextension-window-titler) (for giving each window a unique title).
- Hyprland (for the provided script).
- Jq (for JSON manipulation).
- Socat (for handling IPC communication).

## Steps
- Install the Window Titler extension and set each window to Primary, Secondary, Tertiary, and so on.
- Go into Window Titler Preferences and remove the Opening/Closing tags but keep a white space in the closing tag for read-ability.
  - Keep the Profile title settings default.
- If you're using Hyprland you can use `hyprctl clients` to see that each Firefox window has a different title Starting with Primary/Secondary/Tertiary and ending with - Firefox (May say the name of your Firefox fork).
- Now download the bash script I provided and edit it as you wish. 
  - Remove excess windows or add more.
  - Change workspace names. 
  - Change the browser name. 
  - Edit the event handler if you're not using Hyprland.
- Before running the script, use the command `chmod u+x` to make it executable.
- Now you can make it automatically run by executing the bash command in your Hyprland config.


# If You Found This Guide Helpful At All Please Leave A Star <3
