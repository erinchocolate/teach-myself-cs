# ⚙️Version Control (Git)

## What to study - resources I find helpful📚

- Basic commands 
  - [Git Tutorial for Beginners](https://www.youtube.com/watch?v=DVRQoVRzMIY)
- Advanced commands
  - [13 Advanced (but useful) Git Techniques and Shortcuts](https://www.youtube.com/watch?v=ecK3EnyGD8o)
  - [How to Undo Mistakes With Git Using the Command Line](https://www.youtube.com/watch?v=lX9hsdsAeTk)
- How Git works 
  - [MIT Missing Semester: Version Control(Git)](https://missing.csail.mit.edu/2020/version-control/)
  - [How to explain git in simple words](https://xosh.org/explain-git-in-simple-words/)
  - [Pro Git](https://git-scm.com/book/en/v2)
- Git practice
  - [Git for Professionals Tutorial](https://www.youtube.com/watch?v=Uszj_k0DGsg&t=2049s)
  - [How to Write a Git Commit Message](https://cbea.ms/git-commit/)
- Write your own Git
  - [Write yourself a Git](https://wyag.thb.lt/)



## Study Note ✍️

- [How Git Works](#How Git Works)
- [Git commands](#Git commands)
- [Github](#Github)
- [Branch Strategy](#Branch Strategy)



## How Git Works

### Data model (pseudocode)

```
// a file is a bunch of bytes
type blob = array<byte>

// a directory contains named files and directories
type tree = map<string, tree | blob>

// a commit has parents, metadata, and the top-level tree
type commit = struct {
    parents: array<commit>
    author: string
    message: string
    snapshot: tree
}

```

### Objects and content-addressing

Blobs, trees, and commits are unified in this way: they are all objects. When they reference other objects, they don’t actually *contain* them in their on-disk representation, but have a reference to them by their hash.

```
//An “object” is a blob, tree, or commit
type object = blob | tree | commit

//all objects are content-addressed by their SHA-1 hash
objects = map<string, object>

def store(object):
    id = sha1(object)
    objects[id] = object

def load(id):
    return objects[id]
```

### Reference

```
references = map<string, string>

def update_reference(name, id):
    references[name] = id

def read_reference(name):
    return references[name]

def load_reference(name_or_id):
    if name_or_id in references:
        return load(references[name_or_id])
    else:
        return load(name_or_id)
```

### Repositories

Git *repository* is the data `objects` and `references`.

### Staging area

It's why we have `git add` and `git commit` two separate commands.



## Git commands

### Basic

- `git help` 
- `git init` 
- `git status` 
- `git add <filename>` 
- `git commit` 
- `git log` 
- `git log --all --graph --decorate` - visualize log history
- `git diff <filename>` - show changes relative to the staging area
- `git diff <revision> <filename>`
- `git checkout`

### Branching and merging

- `git branch`
- `git branch <name>`
- `git chekout -b <name>`
- `git merge <revision>` - merges into current branch
- `git mergetool`
- `git rebase` - rebase set of patches onto a new base
- merge v.s rebase
  - [When do you use Git rebase instead of Git merge?](https://stackoverflow.com/questions/804115/when-do-you-use-git-rebase-instead-of-git-merge)

### Remotes

- `git remote`
- `git remote add <name> <url>`
- `git push <remote> <local branch>:<remote branch>`
- `git branch --set-upstream-to=<remote>/<remote branch>`
- `git fetch`
  - [What is the difference between 'git pull' and 'git fetch'](https://stackoverflow.com/questions/292357/what-is-the-difference-between-git-pull-and-git-fetch)
- `git pull`
- `git clone`

### Undo

- `git commit --amend`
- `git reset HEAD <file>`
- `git checkout -- <file>`

### Advanced

- `git config`
- `git add -p` - interactive staging
- `git blame` - show who last edited which line
- `git stash`- temporarily remove modifications to working directory
  - [Git Tutorial: Using the Stash Command](https://www.youtube.com/watch?v=KLEDKgMmbBI&list=PL-osiE80TeTuRUfjRe54Eea17-YfnOOAx&index=4)
- `git bisect`
- `.gitignore`
- merge conflicts
  - Merge conflicts happens when integrating commits from different sources
  - How to undo a conflict and start over: `git merge --abort` or `git rebase --abort`
  - How to solve a conflict: simply clean the file and commit



## Github

- Pull request
  - Without a Pull Request, you would jump right to merging your code
  - A Pull Request invites reviewers to provide feedback before merging
  - Pull Request offers a chance to contribute code to other repositories
  - Pull Request is based on branch not single commit
- Fork
  - Creating a Fork of the original repository, where you can make changes and suggest those changes to be included via a Pull Request
- Github Action
  - [5 Ways to DevOps-ify your App](https://www.youtube.com/watch?v=eB0nUzAI7M8)



## Branch strategy

- Git flow

- Github flow
