# nnreddit
A Reddit backend for the [Gnus newsreader](http://www.gnus.org/).

NOTE: currently for reading only, login and posting not yet implemented.

## Usage

Add these lines to your `.emacs` or `.gnus` file:
```lisp
(require 'nnreddit "/path/to/nnreddit.el")
(add-to-list 'gnus-secondary-select-methods
             '(nnreddit ""))
```

Then subscribe to a group from within Gnus, either by pressing 'U' in the Group buffer and entering "nnreddit:some-subreddit", or with the following command:
```lisp
(gnus-group-unsubscribe-group "nnreddit:some-subreddit")
```

You can also browse individual threads (or sub-threads) with the following syntax:
```lisp
;; Single thread
(gnus-group-unsubscribe-group "nnreddit:some-subreddit/comments/link-id")
;; Sub-thread
(gnus-group-unsubscribe-group "nnreddit:some-subreddit/comments/link-id/comments/comment-id")
```
In other words, simply take the URL of any Reddit thread, replace "ht<b></b>tps://www.reddit.com/r/" with "nnreddit:" and subscribe to that in Gnus.

Alternatively, you can subscribe to a thread or sub-thread directly from the summary buffer with the `nnreddit-subscribe-to-thread' command.

## Screenshots

<a href="https://raw.githubusercontent.com/paul-issartel/nnreddit/master/screenshot.png"><img src="https://raw.githubusercontent.com/paul-issartel/nnreddit/master/screenshot.png" alt="Screenshot of a Reddit link article in Gnus" width="500"/></a>

<a href="https://raw.githubusercontent.com/paul-issartel/nnreddit/master/screenshot2.png"><img src="https://raw.githubusercontent.com/paul-issartel/nnreddit/master/screenshot2.png" alt="Screenshot of a Reddit comment in Gnus" width="500"/></a>
