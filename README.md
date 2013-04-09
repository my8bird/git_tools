git_tools
=========

Tools I use day to day to make git easier.  Basically, this are custom git commands that do specific things to help me out.

Note: Even though these commands are shell scripts they still work on windows becuase git ships with an interpreter.

Installation
============
Clone this repository and puts it contents in your path.

Commands
========

update
------
`git update`

Places all commits on the current branch on top of the most recent HEAD of `master`.  Interactive rebase is used to allow cancelling if something goes weird.

recent
------
`git recent`

List all branches sorted by more recently changed.  I like this because it helps me find the most likly branches I want to switch to instead of just all available choices.

consolidate
-----------
`git consolidate`

Interactive rebase of all commits since your current branch diverged from `master`.  In my flow I make a bunch of commits marked with common tags, think "XXX task 1".  Then when I have a good unit of work finished I use `git consolidate` to move the commits into different buckets.


