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

i3wm starts in *default* mode where the only keybinding is $mod+space, which is used to switch to other modes. The default mode is ideal for interacting with the focused application. Since no keybinding are defined except $mod+space, you can define any keybinding you need in your application without worrying about them colliding with i3wm keybindings.

Interact with i3wm by switching to an appropriate mode. To do that, type `$mod+space`. This will send you to the "mode switching" mode, from which you can jump to other modes.

Modes are self explanatory. When you are in a mode, the keybindings offered by the mode are displayed in the status bar.

From any mode you can type `space` to return to the "mode switching" mode. This means that you can go to navigation mode to select a window you want to move, switch to *move container* mode to move the window, switch again to *resize* mode to give it the size you want, then switch to the *layout* mode to split the container vertically, and switch to the *launcher* mode to open a new terminal in the splitted container. The type `Escape` or `Return` to go back to the default mode and start typing commands in your terminal.

In any mode, use `Escape` or `Return` to leave the mode and go back to the default mode. Some modes excplicitly use the `Return` key for other purposes.

# Installation

Copy `config_modal_bepo` to your i3wm configuration file.

The launcher mode uses the script `dmenu_run_history` [https://tools.suckless.org/dmenu/scripts/dmenu_run_with_command_history/]() and `dmenu_paste_history` which need to be in `$PATH`.


# Configuration

Adapt to your keyboard layout. Most keybindings are mnemonic, e.g. `n` for navigate, `r` for resize... and should work for most keyboard layout. Those which will need to be adapted are the movement keys (ctsr for the bépo layout, hjkl for qwerty, ...)

Edit the variables in the `# Applications` section of the configuration file.

