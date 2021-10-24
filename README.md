# My List of Terminal Command Aliases

## By [Dan Blevins](https://www.linkedin.com/in/dan-blevins/)

<br>

Thanks for reading! Feel free to comment and let me know if you want YouTube tutorials.

Want to stay in touch? Connect with me on [LinkedIn](https://www.linkedin.com/in/dan-blevins/)!

<br>

### Table of Contents
- <a href="#why" style="color: #d4d4d4;">Why Use Aliases?</a>
- <a href="#how" style="color: #d4d4d4;">How do you Make an Alias using a Mac?</a>
- <a href="#list" style="color: #d4d4d4;">My List of Terminal Command Aliases</a>

<br>
<br>

**<a id="why"></a>Why Use Aliases?**

In general, it's important for developers to be lazy and save time when possible. Therefore, aliases are custom keyboard shortcuts that help you save time. For example, it's typically good practice to write comments with your git commits, but it's annoying to constantly type out "git commit -m 'your message comment'." Instead, you can make an alias like `alias gc='git commit -m '` which allows you to simply run "gc 'your message comment'".

I understand it doesn't save you much time, but the more efficient aliases you make, the more time you'll save. As Kevin Malone from The Office puts it: [*Many small time make big time.*](https://getyarn.io/yarn-clip/e2270076-ab06-4d61-8a2f-baf994bfe34f)

<br>

**<a id="how"></a>How do you Make an Alias using a Mac?**

If you're using Mac, open your terminal and run: `echo $0`.
  - If "-bash" prints out, then open your bash profile by running `nano ~/.bash_profile`
  - If "-zsh" prints out, then open your zshrc file by running `nano ~/.zshrc`

Finally, let's add a simple alias in your bash_profile or zshrc file.

Somewhere convenient in your terminal (maybe the very top or the very bottom of your file), type:
```bash
# Terminal Commands
alias cl='clear'
```

Next, save and exit the file by typing: CTRL + X, y (for yes), then press the Enter key.

Finally, save/refresh the changes so they appear in the terminal by running `source ~/.bash_profile` or `source ~/.zshrc`.

Now, you should be able to clear the terminal screen by running `clear` or using your alias by running `cl`.

<br>

**<a id="list"></a>My List of Terminal Command Aliases**

```bash
# Terminal Commands
alias nb='code ~/.bash_profile'
alias sb='source ~/.bash_profile'
alias cl='clear'
alias ls='ls -GFh'
alias ..='cd ..'
alias mkdir='mkdir -v'
alias nano='nano -c $1'
alias hist='history | grep $1'

# Github Commands
alias gs='git status'
alias gba='git branch -a'
alias gpl='git pull'
alias gch='git checkout'
alias gcb='git checkout -b $1'
alias ga='git add '
alias gaa='git add .'
alias gc='git commit -m $1'
alias gsu='git branch --set-upstream-to origin master'
alias gp='git push'
alias gr='git rebase -i'
alias gph='git push heroku HEAD:master'
```
