projectile + speedbar
========

## Summary

This package sits on top of speedbar and projectile and provides an easy
to use and useful integration between the two.

With this package when you switch between projects that work with
projectile, speedbar will automatically show the directory listing of
that project as well as expand the tree to show the file in the project.

## Dependencies

Features that are required by this library: `speedbar` `sr-speedbar`
`projectile`

## Installation

### Melpa

This package is available to install via Melpa. First, make sure the
Melpa package archive is available.

``` lisp
(require 'package)
(add-to-list 'package-archives '("melpa" . "http://melpa.org/packages/"))
```

Then, install this package:

``` lisp
(package-install 'projectile-speedbar)
```

### Manual

Copy speedbar-projectile.el to your load-path and add this to ~/.emacs

    (require 'projectile-speedbar)

To invoke this function manually:

    `projectile-speedbar-open-current-buffer-in-tree

## Customizations

Sometimes, when I am deep in a project tree, I like to use this shortcut
to see full context:

    (global-set-key (kbd "M-<f2>") 'projectile-speedbar-open-current-buffer-in-tree)

You can also disable the feature completely:

    (setq projectile-speedbar-projectile-speedbar-enable nil)

