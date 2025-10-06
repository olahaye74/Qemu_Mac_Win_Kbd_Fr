# Qemu_Mac_Win_Kbd_Fr
Files needed to have a French keyboard on a qemu Windows guest running on a Macbook.

- KBDMacFR.klc.orig Source File to work with.
- KBDMacFR.klc      File saved by MSKLC (V1.4)
- keymap-fr-macbook keymap file for qemu generated with qemu-keymap
- WinKBD.html web tool to help debugging scancodes, ISO codes , VK_ names (bugguy, but still usefull)

1/ Copy keymap-fr-macbook as /opt/homebrew/Cellar/qemu/10.1.0/share/qemu/keymaps/fr-mac (adpat path and keymap name to you installation)

2/ Start your Windows and install the keyboard package.
If you want to build your own kbd installer:
- start control panel -> Programs & Options -> Add/Remove components -> Enable .Net v3.5
- Install MSKLC https://www.microsoft.com/en-us/download/details.aspx?id=102134
- load KBDMacFR.klc
- Menu project / Build DLL and Setup Package

3/ Win-I (Parameters)
 - Time @ Language -> Language and region right click on the  3 dots -> linguistic options
 - Add a keyboard -> Choose Français (Macbook, AZERTY)

 You're done.
