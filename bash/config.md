# config path
    ~/.bashrc
> execute at any (virtual)terminal startup
```
~/.bash_profile
```
> only exec at login
# environment variables
* mostly define in ~/.bash_profile
* define in ~/.profile to compatible with other shells
```bash
export $VAR=$value
```
# configs
## history
```bash
export HISTCONTROL="erasedups:ignorespace"
```
> not showing repeated commands
## auto cd
```bash
shopt -s autocd
```