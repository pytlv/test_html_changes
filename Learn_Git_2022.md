# Learn Git in 15 minutes
Learn Git in 15 minutes [Notion] (https://www.notion.so/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049)
PS D:\code_22\learn_git> git init
Initialized empty Git repository in D:/code_22/learn_git/.git/

# Markdown
Bold    **        **Text** 
Italic  *       	*Text* \
Strike ~~         ~~Text~~
Strikethrough   	~~ ~~
Code (inline)	`` `Statement`
This site was built using [GitHub Pages](https://pages.github.com/).


===
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        f

nothing added to commit but untracked files present (use "git add" to track)
# Configuring git
git config --global user.name "Barak"
git config --global user.email "herzman@gmail.com"

## Listing Congiuration
git config --get user.email
###  viewing the entire config, the correct argument is --list, not --get-all (or you may also want --edit).

*$ git config --global --list*
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
user.name=Barak
user.email=herzman@gmail.com

=== Problems
1] Stuck in CLI
To interrupt the current command press CTRL-C.
If the bottom-left of your shell window shows --More-- you are viewing a file using more.
To exit from more press q.
=
