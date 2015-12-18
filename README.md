# DiffView for Sublime Text 3
*Git and SVN Diff Viewer for Sublime Text 3*

## Usage
* `Alt + Shift + D` to run a diff
    * *See below for supported diff options*
    * This lists all the changed hunks, and shows you a preview as you move down the list
    * You can search for a particular file in the list of hunks, which will filter the results
    * Hit `Enter` to jump to the currently selected diff
    * hit `Esc` to cancel the Diff View, and return to where you were
* `Alt + D` to review the last diff
    * This will show the list of hunks from the last diff, starting from the last hunk you selected

## Supported Diff Options

### Git
* *Default* (when there's no input): comparison of wc against `HEAD` - i.e. show unstaged changes
* `HEAD` or `branch` or `SHA` or `tag`: compare wc against `HEAD`/`branch`/`SHA`/`tag`
* `branch..` compare `branch` with wc
* `..branch` compare wc with `branch`
* `branch_a..branch_b` compare `branch_a` with `branch_b`
* `branch...` compare the merge-base of wc and `branch` with wc
* `branch_a...branch_b` compare the merge-base of `branch_a` and `branch_b` with `branch_b`

### SVN
* *Default* (when there's no input): show uncommitted changes
* `-r 123` compare revision 123 with the working copy
* `-c 234` show changes made in commit 234
