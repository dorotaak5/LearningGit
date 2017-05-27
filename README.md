## This will be a git learning center

## Version Control System (VCS)
a system that records changes to a file or set of files over time so that you can recall specific versions later.

## RCS
 RCS works by keeping patch sets (that is, the differences between files) in a special format on disk; it can then re-create what any file looked like at any point in time by adding up all the patches.

## Centralized Version Control Systems
Centralized Version Control Systems (CVCSs) were developed. These systems, such as CVS, Subversion, and Perforce, have a single server that contains all the versioned files

## Distributed Version Control Systems
This is where Distributed Version Control Systems (DVCSs) step in. In a DVCS (such as Git, Mercurial, Bazaar or Darcs), clients don’t just check out the latest snapshot of the files: they fully mirror the repository.

## Git has three main states that your files can reside in:

.Committed means that the data is safely stored in your local database

.Modified means that you have changed the file but have not committed it to your database yet.

.Staged means that you have marked a modified file in its current version to go into your next commit snapshot.

## Git project:

.Git directory(repository)
  .is where Git stores the metadata and object database for your project

.Working tree
  .is a single checkout of one version of the project

.Staging area
  .is a file, generally contained in your Git directory, that stores information about what will go into your next commit

## First-Time Git Setup

You should have to do these things only once on any given computer; they’ll stick around between upgrades. You can also change them at any time by running through the commands again.

git config --global user.name "Herman Soto"
git config --global user.email "hermansoto@me.com"
git config --global push.default matching
git config --global alias.co checkout

git config --list
git config user.name


## Initializing a Repository in an Existing Directory
go to your
git init

git clone [url]

## Checking the Status of Your Files

git status 
git -s
git -s --short
git diff ## is for only unstaged
git diff --staged
git diff --cached

## Tracking New Files

git add <file>
git add <dir>
git add -a -m "my description"

## git add command is a multipurpose command – you use it to:

.begin tracking new files
.to stage files
.and to do other things like marking merge-conflicted files as resolved.

## Committing Your Changes

git commit
git commit -m "comment"

## Removing Files

git rm
git rm --cached README

## You can pass files, directories, and file-glob patterns to the git rm command. That means you can do things such as:

$ git rm log/\*.log

## Moving Files 

git mv app.js app.json  //(rename)

## However, this is equivalent to running something like this:

$ mv README.md README
$ git rm app.js
$ git add app.json

## Viewing the Commit History

git clone https://github.com/schacon/simplegit-progit

git log

git log -p -2

git log --stat

git log --pretty=oneline

## udemy 48 using git

ls -a
git status
git add . ()
git rm --cached -r <folder or file>
git commit -a -m ""

## 

.gitignore 

<file or folder name>

