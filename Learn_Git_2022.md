# Learn Git in 15 minutes
Learn Git in 15 minutes [Notion] (https://www.notion.so/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049)
PS D:\code_22\learn_git> git init
Initialized empty Git repository in D:/code_22/learn_git/.git/

Software Carpentry [SW Carpentry exiting command line]
(https://hpcarcher.github.io/2014-12-03-edinburgh/novice/ref/05-prompts-exits.html#:~:text=To%20interrupt%20the%20current%20command,viewing%20a%20file%20using%20less%20.)

# Markdown
Bold    **        **Text** 
Italic  *       	*Text* \
Strike ~~         ~~Text~~
Strikethrough   	~~ ~~ \
Code (inline)	`` `Statement` \
This site was built using [GitHub Pages](https://pages.github.com/). 

# git  Problems 
1] Stuck in CLI
To interrupt the current command press `CTRL-C`.
If the bottom-left of your shell window shows --More-- you are viewing a file using more.
To exit from more press `q`.
=


# git commands

# Configuring git
`git config --global user.name "Barak"`
`git config --global user.email "herzman@gmail.com"`

## Listing Congiuration
`git config --get user.email`
###  viewing the entire config, the correct argument is --list, not --get-all (or you may also want --edit).

```$ git config --global --list`
	filter.lfs.process=git-lfs filter-process
	filter.lfs.required=true
	filter.lfs.clean=git-lfs clean -- %f
	filter.lfs.smudge=git-lfs smudge -- %f
	user.name=Barak
	user.email=herzman@gmail.com
```
```$ git status
	On branch master
	No commits yet
	Untracked files:
	(use "git add <file>..." to include in what will be committed)    
	nothing added to commit but untracked files present (use "git add" to track) 
```

` git add .\Learn_Git_2022.md`
``` git status
On branch master
	No commits yet
	Changes to be committed:
	  (use "git rm --cached <file>..." to unstage)
			new file:   Learn_Git_2022.md
```
**Changed Learn_Git_2022.md			**
```On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Learn_Git_2022.md
*modified in red*
```
==> 
`git add Learn_Git_2022.md`
```git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   Learn_Git_2022.md
*modified in green*
```
**add all files in a directory**
`git add .`

**commit**
`git commit -m "Commit message"`
```
	[master (root-commit) 3a2b0fc] 1st commit
	 1 file changed, 45 insertions(+)
	 create mode 100644 Learn_Git_2022.md
```

*commit  history* 
`git log`
```
git log
	commit 0bd45212232fd02e2602033851141e2d51bd987c (HEAD -> master)
	Author: Barak <herzman@gmail.com>
	Date:   Wed Dec 21 10:17:37 2022 +0200

		2nd commit

	commit 3a2b0fcf012369da59032df3ead46a8d23f6d536
	Author: Barak <herzman@gmail.com>
	Date:   Wed Dec 21 10:04:59 2022 +0200

		1st commit
``` 
