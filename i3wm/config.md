# config path
    ~/.config/i3/config
# configures
## keybinding
    bindsym $key $action
    bindsym $mod+x exec i3lock
* $key
    * special key: XF86Audio...
    * combined key: $mod+Shift+x ...
* $action
    * internal
        * focus $direction : change currently focused window to $direction
            * $direction: up / down / left / right /(parent /child for floating window)
        * kill : close focused window
        * move $direction : exchange position with window $direction
        * split $way : allocate position for opening a new window
            * $way : h for horizontal / v for vertical
        * layout $way : change layout for current desktop
            * $way : stacking / tabbed / toggle split
        * floating (toggle) : change current window into float(toggle for toggle between floating and tiling)
        * restart : just treat it as "refresh" in Windows, trigger it after editing config file or after an error has occured.
    * external
        * exec $param $command : in # actions
## variable setting
    set $var_name(including $) $value
    set $bg-color #000000
* looks like a environmental variable, haven't tried yet.
## customising
    gaps $method $value
    gaps inner 10
* $method : outer(between window frame to edges) / inner(between windows)
```
default_orentation $method
```
* $method : auto / vertical / horizontal
```
default_border $method $value
```
> only works in tiling windows
* $method : pixel(no title bar) / none(no border)
```
default_floating_border
```
> only works in floating windows
```
assign $rule $workspace
```
* $rule: [class="$class_name"]
    > you may look up for class_name using command "xprop"
* font pango:$font_name $font_size
# actions
    exec $param $command
* $param(optional) : --nostartup-id
* $command : any command you may use in shells connecting commands using "&&" is allowed
