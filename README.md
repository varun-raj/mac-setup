### My Mac Setup

#### Symblink ZSH Files

```sh
rm ~/.zsh_history && ln -s /Users/varunraj/Library/Mobile\ Documents/com\~apple\~CloudDocs/DevSetup/Bash/.zsh_history ~/.zsh_history
rm ~/.zshrc && ln -s /Users/varunraj/Library/Mobile\ Documents/com\~apple\~CloudDocs/DevSetup/Bash/.zshrc ~/.zshrc
```

#### Alias

```sh
# Git Shortcuts
alias gcb='git checkout -b $1'
alias gcm='git checkout main'
alias gpm='git pull origin main'
alias gc='git checkout $1'
alias gpc='git pull origin $(git branch --show-current)'

# HN Dev Shortcuts
alias nr='npm run dev' # NextJS Project Start
alias c='code .' # To Open VS Code

# React Scripts
alias rs='npm run start'
alias rb='npm run build'

# General
alias sz='source ~/.zshrc'
alias cz='code ~/.zshrc'
alias cl='clear'

# Find and delete .DS_Store Files
alias cleanup="find . -type f -name '*.DS_Store' -ls -delete"

# Empty Trash and Other Caches
alias emptytrash="sudo rm -rfv ~/Library/Caches/; sudo rm -rfv /Volumes/*/.Trashes; sudo rm -rfv ~/.Trash; sudo rm -rfv /private/var/log/asl/*.asl; sqlite3 ~/Library/Preferences/com.apple.LaunchServices.QuarantineEventsV* 'delete from LSQuarantineEvent'"

# Update everything at once
alias brewup='brew update && brew upgrade && brew cu -a -f --cleanup -y && brew cleanup; brew doctor'

```
