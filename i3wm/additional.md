# additional packages for better experience
## terminal simulators
1. xterm
    * pros:
        1. light
        2. ship with xorg
    * cons:
        1. terrible in customizing
2. konsole
    * pros:
        1. rich color presets
        2. easy to customize
    * cons:
        1. no animation settings
        2. uncancelable toolbar - bad at tiling
        3. too heavy - complex dependency in kde
3. kitty
    * pros:
        1. not heavy
        2. gpu support
        3. animation
        4. easy to customize
    * cons:
        1. not as light
        2. repeative function with wms - tabs
        3. terrible support for tmux and so
## display managers
1. sddm
    * pros:
        1. fancy themes
        2. light
    * cons:
        1. buggy when working with wms
2. lightdm
    * pros:
        1. light
        2. easy to config
    * cons:
        1. not fancy
        2. splashes at boot
## status bars
1. i3status
    * pros:
        1. ship with i3wm
        2. light
    * cons:
        1. not fancy
        2. not modular
2. i3blocks
    * pros:
        1. light
        2. modular
        3. easy to write scripts
    * cons:
        1. default setting zero ready to use
        2. not fancy
3. polybar
    * pros:
        1. fancy & ready to use
        2. weak connection with i3wm
        3. modular
    * cons:
        1. not light
        2. not compatible with i3bar
## audio manager
1. pulseaudio
    * pros:
        1. powerful
        2. ready to use
    * cons:
        1. some times laggy
2. jack
    * pros:
        1. high quality
    * cons:
        1. bad compability
3. alsa
    * pros:
        1. stable
    * cons:
        1. outdated
4. pipewire
    * pros:
        1. compatible with all above
        2. video supports
    * cons:
        1. complex configuration
## notification
1. dunst
## file manager
1. yazi
    * pros:
        1. ready to use
        2. fast
        3. vim commands
    * cons:
        1. heavy dependency
2. dolphin
    * pros:
        1. easy to mount drives
    * cons:s
        1. even heavier dependency - kde
## hardware control
1. backlight control : brightnessctl/xbacklight
2. bluetooth control ui : bluetui
3. network connection ui : nmtui
4. power control : tlpui
