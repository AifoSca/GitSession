
# GitSession

## What is Git?

Distributed Version Control System (DVCS)

These systems do not necessarily rely on a central server to store all the versions of a project file.

In Distributed VCS, every contributor has a local copy or “clone” of the main repository i.e. everyone maintains a local repository of their own which contains all the files and metadata present in the main repository.

[Reference](https://www.quora.com/What-is-Git-and-why-should-I-use-it)

### Diference between Working Tree, Local and Remote repository

- Working Tree: Where code changes are made

- Local Repository: Commit command happens

- Remote Repository: Push, Pull command happen


### What Origin means?

**ORIGIN**  is an **alias**  *_on your system_* for a particular remote repository. It's not actually a property of that repository.

    [ ~/GitSession ]
    $ git remote -v      # show the name for the remote branch/repo
    origin  https://github.com/AifoSca/GitSession.git (fetch)
    origin  https://github.com/AifoSca/GitSession.git (push)

    ### How can you push in this situation
    $ git push origin master 
    or
    $ git push https://github.com/AifoSca/GitSession.git master

    ### Renaming the remote repository
    [ ~/GitSession ]
    $ git remote rename origin remote_repo    # to change the name
    [ ~/GitSession ]
    $ git remote -v
    remote_repo     https://github.com/AifoSca/GitSession.git (fetch)
    remote_repo     https://github.com/AifoSca/GitSession.git (push)
    
    ### How can you push in this situation
    $ git push remote_repo master
    or
    $ git push https://github.com/AifoSca/GitSession.git master


## Git Basic commands!!
| Git Command | 	Explanation											    |
| --------   |--------------------------------------------------------------|
| git init   | 	 Initialize Local Git repository                            |
| git config  --global user.name 'your.name' | 	Adds name   |
| git config --global user.email 'your.email' |	Adds email |
| git add	 | Add Files to index |
| git status |	Check the status of Working Tree|
| git commit |	Commit Changes In Index  |
| git push	 | Push to Remote repository  |
| git pull	 | Pull latest from remote repository |
| git clone	 | Clone repository into a new directory |
| git log    | lists commit log |
| git diff 	 | difference between |



## .gitignore?...and what about git stash?

## Merge vs Rebase

## Revert and Reset

## Cherry-pick
