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

------------------

```bash
$ git init
```

Initializes an empty local repository

------------------

```bash
$ git status
```

Show the state of the current branch (changes without a _commit_)

------------------

```bash
$ git clone <url> <directory>
```

Makes a local copy of a remote repository (at _url_) in _directory_

------------------

```bash
$ git add <file>
```

Adds a file to the repository index (_working directory_ -> _staging area_)

------------------

```bash
$ git commit -m <message>
```

Makes a new commit (_staging area_ -> _repository_)

------------------

```bash
$ git push <remote-name> <branch>
```

Updates remote objects with changes in the local objects

------------------

```bash
$ git fetch <remote-name> <branch>
```

Downloads changes from _branch_ in _remote-name_

------------------

```bash
$ git merge <branch>
```

Combines the changes in _branch_ with the current branch

------------------

```bash
$ git pull <remote-name> <branch>
```

It performs the following:

```bash
$ git fetch <remote-name> <branch> 

$ git merge <remote-name>/<branch>
```

------------------

```bash
$ git branch <new-branch>
```

Creates a new _branch_ which points to the current _HEAD_

------------------

```bash
$ git tag <new-tag> <commit>
```

Creates a new _tag_ to identify a particular _commit_. If no _commit_ is given, the current (_HEAD_) is taken

------------------

```bash
$ git checkout [ <branch> | <tag> | <commit> ]
```

Moves the _working pointer_ to a specific point in the repository tree

Special case:

```bash
$ git checkout -b <new-branch>
```

Equivalent to:

```bash
$ git branch <new-branch>

$ git checkout <new-branch>
```

------------------

```bash
$ git log
```

Displays information about the commits

------------------

```bash
$ git show <commit>
```

Displays the changes in modified files on the _commit_. If no _commit_ is given the current (_HEAD_) is taken.

------------------

# Extra

```bash
$ git log --oneline --decorate --graph --all --stat
```

