# i3-modal

*This config file was adapted to the bépo keyboard layout. The same approach can easily be reproduced with any other layout.*

This aim of this configuration file is to avoid the use of the modifier key to reduce wrist strain. There are two modes: the *default* mode to interact with i3wm and an *insert* mode to interact with the focused application.

i3wm starts in *default* mode where the keybindings are like the usual i3 keybindings without the modifier key. For example, to open a terminal, rather than typing `$mod+Enter`, just type `Enter`. 

In this mode, you cannot interact with your applications. When the terminal is open, typing will trigger i3wm keybindings rather than input characters in the terminal. To interact with the applications, you need to switch to *insert* mode by typing `Space`. To switch back to *normal* mode, type `$mod+Space`.

# Installation

Copy `config_modal` to your i3wm configuration file.
