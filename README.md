### Install and config Tmux


#### Requirements

  - tmux **`>= 2.4`** running inside Linux, Mac, OpenBSD, Cygwin or WSL
  - awk, perl and sed
  - outside of tmux, `$TERM` must be set to `xterm-256color`

#### Install dependencies

###### macOS
```console
brew install tmux awk perl sed tmux-mem-cpu-load reattach-to-user-namespace
```
###### Linux

#### Install tmux-mem-cpu-load
```console
brew install tmux-mem-cpu-load
```

#### Install tmux
```console
sudo apt install -y tmux xsel
```

##### Install config Tmux
```console
git clone https://gitlab.com/lucasmartinseti/lmtmux.git ~/.config/lmtmux
```

##### Install oh-my-tmux
```console
git clone https://github.com/gpakosz/.tmux.git ~/.tmux
ln -s -f ~/.tmux/.tmux.conf ~/.tmux.conf
ln -s -f ~/.config/lmtmux/tmux.conf.local ~/.tmux.conf.local
```
