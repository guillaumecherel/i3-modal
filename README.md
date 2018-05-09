# i3-modal

*This config file was adapted to the bépo keyboard layout, but should be adaptable to other layout just by changing the movement keys in the file. In bépo, those are ctsr rather than the standard hjkl.*

This configuration file uses i3wm modes for a twofold purpose: first to avoid the use of the modifier key which requires curling fingers in complicated positions, and second to reduce keybinding collisions between i3wm and other applications (you can define any keybinding in you application without fear of them being used by i3wm already).

The following modes are used: 
- *launcher*: start some applications,
- *navigate*: move focus between containers,
- *move container* in the workspace and between workspaces,
- *layout*: change the current workspace layout,
- *move workspace* between outputs,
- *window resize*,
- *i3 special*: exit i3wm and other special actions.

i3wm starts in *default* mode where the only keybinding is `Super_L`, which is used to switch to other modes. The default mode is ideal for interacting with the focused application. Since no keybinding are defined except `Super_L`, you can define any keybinding you need in your application without worrying about them colliding with i3wm keybindings.

Interact with i3wm by switching to an appropriate mode. To do that, type `Super_L`. This will send you to the "mode switching" mode, from which you can jump to other modes.

Modes are self explanatory. When you are in a mode, the keybindings offered by the mode are displayed in the status bar.

From any mode you can type `Super_L` to return to the "mode switching" mode. This means that you can go to navigation mode to select a window you want to move, switch to *move container* mode to move the window, switch again to *resize* mode to give it the size you want, then switch to the *layout* mode to split the container vertically, and switch to the *launcher* mode to open a new terminal in the splitted container.

In any mode, use `Escape` to leave the mode and go back to the default mode.

`Return` is generally used to execute an action and switch back to default mode. The action depends on the mode. For example, in launcher mode, it launches a terminal. In navigate mode, it executes no action and only returns to default mode.

`space` switches to the current modes "natural" alternate mode, that is the mode that one may naturally switch to from that mode. For example, from the navigate mode, space switches to move container mode.

# Installation

Copy `config_modal_bepo` to your i3wm configuration file.

# Configuration

Adapt to your keyboard layout. Most keybindings are mnemonic, e.g. `n` for navigate, `r` for resize... and should work for most keyboard layout. Those which will need to be adapted are the movement keys (ctsr for the bépo layout, hjkl for qwerty, ...)

Edit the variables in the `# Applications` section of the configuration file to your preference.

