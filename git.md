---
title:
- Git™
author:
- Patricio Iribarne Catella
date:
- January 08, 2020
theme:
- Copenhagen
---

# History

- Linus Torvalds in 2005
- "_The stupid content tracker_"

------------------

# Features

- Branching and Merging
- Small and Fast
- Distributed
- Data Assurance
- Staging Area (`git add` & `git commit`)
- Free and Open Source

------------------

# Commands

## git _init_

Initializes an empty local repository

------------------

## git _status_

Show the state of the current branch (changes without a _commit_)

------------------

## git _clone_ `<url> <directory>`

Makes a local copy of a remote repository (at _url_) in _directory_

------------------

## git _add_ `<file>`

Adds a file to the repository index (_working directory_ -> _staging area_)

------------------

## git _commit_ -m `<message>`

Makes a new commit (_staging area_ -> _repository_)

------------------

## git _push_ `<remote-name> <branch>`

Updates remote objects with changes in the local objects

------------------

## git _fetch_ `<remote-name> <branch>`

Downloads changes from _branch_ in _remote-name_

------------------

## git _merge_ `<branch>`

Combines the changes in _branch_ with the current branch

------------------

## git _pull_ `<remote-name> <branch>`

It performs the following:

`git fetch <remote-name> <branch>` + `git merge <remote-name>/<branch>`

------------------

## git _branch_ `<new-branch>`

Creates a new _branch_ which points to the current _HEAD_

------------------

## git _tag_ `<new-tag> <commit>`

Creates a new _tag_ to identify a particular _commit_. If no _commit_ is given, the current (_HEAD_) is taken

------------------

## git _checkout_ `[ <branch> | <tag> | <commit> ]`

Moves the _working pointer_ to a specific point in the repository tree

------------------

Special case: `git checkout -b <new-branch>`: `git branch <new-branch>` + `git checkout <new-branch>`

------------------

## git _log_

Displays information about the commits

------------------

## git _show_ `<commit>`

Displays the changes in modified files on the _commit_. If no _commit_ is given the current (_HEAD_) is taken.

------------------

# Extra

`git log --oneline --decorate --graph --all --stat`

