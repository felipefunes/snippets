# snippets
[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

## Install RBENV on my mac
Source: [Laila Winner](http://robots.thoughtbot.com/using-rbenv-to-manage-rubies-and-gems)

Remove rvm
`rvm implode`

Restart shell
`exec $SHELL -l`

Install rbenv using homebrew (You need XCode)
`brew update`
`brew install rbenv`

Configure your bash or zsh profile
`echo 'eval "$(rbenv init -)"' >> ~/.zlogin`
`source ~/.zlogin`

Install ruby-build and rbenv rehash gem
`brew install rbenv-gem-rehash`
`brew install ruby-build`

Install your preferred version of Ruby and set it as the global default
`rbenv install 2.0.0-p353`
`rbenv global 2.0.0-p353`

Update to the latest Rubygems version
`gem update --system`

You can set project-specific Ruby and gem versions by running the rbenv local command within your project directory
`rbenv local 2.0.0-p247`



## Create a mysql dump

mysql -u root -ppassword database_name < database_name.sql


