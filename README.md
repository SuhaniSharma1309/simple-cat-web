## Git Hidden Folder
There is a hidden folder called '.git' which tells you that out project is a git repo.

if we want to create a git rep in a new project we create the folder and initialize that repo using 'git init'

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add Readme.md
# make changes to readme.md
git commit -a -m "add readme file"
```

## Cloning
we can clone in three ways: HTTPS, SSH, Github CLI

Since we are using Github Codespaces, we ll create a temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd/workspace/tmp
```

### HTTPS

```sh
git clone https://github.com/SuhaniSharma1309/simple-cat-web.git
cd simple-cat-web/
```

## Commits
when we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.

```sh
git commit
```
Set the global editor

```
git config --global core.editor emacs
```

Make a commit and commit message without opening an editor
git commit -m "add another exclamation"


## Branches

## Remotes

## Stashing

## Merging

## Add
When we want to stage changes that will be included in the commit. we can use the . to add all possible files. 

```
git add Readme.md
git add. 
```

## Reset
Reset allows you to move staged changes to unstaged.
this is useful when you want to revert all files not to be not committed.

```
git add .
git reset
```
> git reset will revert a git add.

## Status
Git status shows you which files will or will not be commited.

```
git status
```

## Gitconfig file
The gitconfig file is what stores your global configurations for git such as email, name, editor and more.
Showing the contents of our .gitconfig file

```
git config --list
```
when you first install git on a machine you are supposed to set up your email and name

``sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```
## Log

git log will show the recent git commits to the git tree

## Push
when we want to push a rep to our remote origin

```
git push
```

