# personal-env

A fairly small project containing things used in my personal environment, and the way I set it up. It's pretty far from complete, but vaguely useful!

## win

Contains an incomplete `setup.todo` - instructions on how to set up my personal environment on windows, focusing on development using Sublime Text 3, MavensMate, and git, using a chain of fun things to ensure that SSL keys are able to be presented when ST3 calls out to cmd (requiring only firing up Pageant and entering passwords on login, rather than for every commit, etc - pt as the ST3 git plugins don't handle entering passphrases for SSL keys when doing git callouts).

## osx

Currently contains only `.bash_profile_pub`: bash_profile elements I commonly use/rely on being set/whatever, that don't contain any sensitive info. Can be imported into your `.bash_profile` with:

```bash
source ~/.bash_profile_pub
```

If you're using the repo as the master, you'll probably want to create a [hard] link to the repo

```bash
cd ~
ln path/to/.bash_profile_pub
```

Creating the hard link to your local repo will allow you to tweak the `.bash_profile_pub` inside the local repo, and have your actual bash profile update automatically wihtout having to shuffle files every time. In addition, once you've loaded it once, you'll also have an alias `reload-bash-profile` that will reload your bash profile on the fly within a terminal session (i.e., executes `. ~/.bash_profile`)
