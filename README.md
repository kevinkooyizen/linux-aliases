# Linux-aliases
Aliases for Linux which includes some Ruby, Rails, PHP, Laravel aliases

# System
alias killall='kill -9 $(lsof -i tcp:3000 -t)'
alias gb='gedit ~/.bashrc'
alias sb='subl .'
alias suu='sudo apt update && sudo apt upgrade'
alias e='exit'

# Ruby
alias rdm='rake db:migrate'
alias rdc='rake db:create'
alias roll='rake db:rollback STEP=1'
alias bi='bundle install'
alias be='bundle exec'
alias rkr='bundle exec rake routes'
alias berdm='bundle exec rake db:migrate'
alias ber='bundle exec rspec'
alias beg='bundle exec guard'

# Rails
alias rar='rails routes'
alias rc='rails console'
alias ras='rails server'
alias rg='rails generate'
alias rgm='rails generate migration'
alias rgc='rails generate controller'
alias seed='rails db:seed'

# Git
alias gphom='git push origin master'
alias gphhm='git push heroku master'
alias gplom='git pull origin master'
alias gc='git commit -m '
alias ga='git add .'
alias gpho='git push origin'
alias gplo='git pull origin'
alias gbh='git branch'
alias gch='git checkout'
alias gcm='git checkout master'
alias gm='git merge'
alias gcb='git checkout -b'
PROMPT_COMMAND='_L="$(history 1)"; [ "$_L" != "$_X" ] || git status && _X="$_L"'

# Heroku
alias hro='heroku open'
alias hrl='heroku logs'
alias hrseed='heroku run rake db:seed'
alias hrfig='figaro heroku:set -e production'

# PHP
alias artm='php artisan migrate'
alias ser='php artisan serve'
alias artroll1='php artisan migrate:rollback --step=1'
alias lpst='sudo /opt/lampp/lampp start'
alias lpsp='sudo /opt/lampp/lampp stop'
alias mysp='sudo service mysql stop'
alias lprs='sudo /opt/lampp/lampp restart'

# Laravel
alias pas='php artisan serve'
alias par='php artisan route:list'
