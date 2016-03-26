# nnreddit
A Reddit backend for the [Gnus newsreader](http://www.gnus.org/).

NOTE: currently for reading only, login and posting not yet implemented.

## Usage

Add this line to your `.emacs` or `.gnus` file:
```lisp
(require 'nnreddit "/path/to/nnreddit.el")
```

Then subscribe to a group from within Gnus, either by pressing 'U' in the Group buffer and entering "nnreddit:some-subreddit", or with following command:
```lisp
(gnus-group-unsubscribe-group "nnreddit:some-subreddit")
```

## Screenshots

<a href="https://raw.githubusercontent.com/paul-issartel/nnreddit/master/screenshot.png"><img src="https://raw.githubusercontent.com/paul-issartel/nnreddit/master/screenshot.png" alt="Screenshot of a Reddit link article in Gnus" width="500"/></a>

<a href="https://raw.githubusercontent.com/paul-issartel/nnreddit/master/screenshot2.png"><img src="https://raw.githubusercontent.com/paul-issartel/nnreddit/master/screenshot2.png" alt="Screenshot of a Reddit comment in Gnus" width="500"/></a>
