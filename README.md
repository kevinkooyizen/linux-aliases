# Linux Aliases

* System
* Ruby
* Rails
* Git
* Heroku
* PHP
* Laravel

# System
alias killall='kill -9 $(lsof -i tcp:3000 -t)'<br>
alias gb='gedit ~/.bashrc'<br>
alias sb='subl .'<br>
alias suu='sudo apt update && sudo apt upgrade'<br>
alias e='exit'<br>

# Ruby
alias rdm='rake db:migrate'<br>
alias rdc='rake db:create'<br>
alias roll='rake db:rollback STEP=1'<br>
alias bi='bundle install'<br>
alias be='bundle exec'<br>
alias rkr='bundle exec rake routes'<br>
alias berdm='bundle exec rake db:migrate'<br>
alias ber='bundle exec rspec'<br>
alias beg='bundle exec guard'<br>

# Rails
alias rar='rails routes'<br>
alias rc='rails console'<br>
alias ras='rails server'<br>
alias rg='rails generate'<br>
alias rgm='rails generate migration'<br>
alias rgc='rails generate controller'<br>
alias seed='rails db:seed'<br>

# Git
alias gphom='git push origin master'<br>
alias gphhm='git push heroku master'<br>
alias gplom='git pull origin master'<br>
alias gc='git commit -m '<br>
alias ga='git add .'<br>
alias gpho='git push origin'<br>
alias gplo='git pull origin'<br>
alias gbh='git branch'<br>
alias gch='git checkout'<br>
alias gcm='git checkout master'<br>
alias gm='git merge'<br>
alias gcb='git checkout -b'<br>
alias gd='git diff'<br>
alias gr='git reset'<br>
<br>
~ The next line runs git status on press of enter key ~<br>
PROMPT_COMMAND='_L="$(history 1)"; [ "$_L" != "$_X" ] || git status && _X="$_L"'<br>

# Heroku
alias hro='heroku open'<br>
alias hrl='heroku logs'<br>
alias hrseed='heroku run rake db:seed'<br>
alias hrfig='figaro heroku:set -e production'<br>

# PHP
alias artm='php artisan migrate'<br>
alias ser='php artisan serve'<br>
alias artroll1='php artisan migrate:rollback --step=1'<br>
alias lpst='sudo /opt/lampp/lampp start'<br>
alias lpsp='sudo /opt/lampp/lampp stop'<br>
alias mysp='sudo service mysql stop'<br>
alias lprs='sudo /opt/lampp/lampp restart'<br>

# Laravel
alias pas='php artisan serve'<br>
alias par='php artisan route:list'<br>
