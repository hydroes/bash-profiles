# bash-profiles
my config settings for zsh / oh-my-zsh


export SHELL=/bin/zsh
export ZSH=$HOME/.oh-my-zsh
export EDITOR=/usr/bin/vi
ZSH_THEME="robbyrussell"

plugins=(git, zsh-nvm)

export PATH="/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:$HOME/.rvm/bin"
export GOPATH="$HOME/go"

fpath=(/usr/local/share/zsh-completions $fpath)

source $ZSH/oh-my-zsh.sh

source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh

[[ -s $(brew --prefix)/etc/profile.d/autojump.sh ]] && . $(brew --prefix)/etc/profile.d/autojump.sh

# eval "$(direnv hook zsh)"

# # Add RVM to PATH for scripting. Make sure this is the last PATH variable change.
# export PATH="$PATH:$HOME/.rvm/bin"

alias gs='git status'
alias ga='git add -p'
alias gb='git branch -a'
alias gpl='git pull'
alias gplr='git pull -r'
alias gps='git push'
alias gc='git commit -m'
alias gco='git checkout'
alias gcl='git clone'
alias gl='git log --oneline'
alias gd='git diff'
alias gf='git fetch'

alias l='ls -la'

alias gitpass='echo "JS/YbyaNJUMUg9eS+cSXk86mKXIQT4RX9kD3j3pKuA" | pbcopy'


