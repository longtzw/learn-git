## Showing Your Remotes

`$ git remote`

If you’ve cloned your repository, you should at least see **origin** that is 
the default name Git gives to the server you cloned from.

You can also specify -v, which shows you the URLs that Git has stored for the 
shortname to be used when reading and writing to that remote.

`$ git remote -v` 

## Adding Remote Repositories

`git remote add <shortname> <url>`

## Fetching and Pulling from Your Remotes

As you just saw, to get data from your remote projects, you can run:

`$ git fetch [remote-name]`

如果执行 `git clone <url>` 命令 git 将自动执行 `git remote add origin <url>`。

So, git fetch origin fetches any new work that has been pushed to that server 
since you cloned (or last fetched from) it.

**It’s important to note** that the git fetchcommand only downloads the data 
to your local repository. it doesn’t automatically merge it with any of your 
work or modify what you’re currently working on. You have to merge it manually 
into your work when you’re ready.

## Pushing to Your Remotes

`$ git push [remote-name] [branch-name]`

> 其实 remote-name 就是 remote repository url 在 local repository 中的别名。

> 同一个 local repository 中的内容可以被 push 到不同的 remote repository。

## Inspecting a Remote

`$ git remote show [remote-name]`

The command helpfully tells you that if you’re on the master branch.

## Removing and Renaming Remotes

`$ git remote rename [src-remote-name] [dst-remote-name]`

`$ git remote rm [remote-name]`

