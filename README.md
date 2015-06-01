projectile + speedbar
========

## Summary

This package sits on top of speedbar and projectile and provides an easy
to use and useful integration between the two.

With this package when you switch between projects that work with
projectile, speedbar will automatically show the directly listing of
that project as well as expand the tree to show the file in the project.

Features that might be required by this library: `speedbar'
`sr-speedbar' `projectile'

To invoke this function manually:

    `projectile-speedbar-open-current-buffer-in-tree

## Installation

Copy speedbar-projectile.el to your load-path and add this to ~/.emacs

    (require 'projectile-speedbar)

## Customizations

Sometimes, when I am deep in a project tree, I like to use this shortcut
to see full context:

    (global-set-key (kbd "M-<f2>") 'projectile-speedbar-open-current-buffer-in-tree)

You can also disable the feature completely:

    (setq projectile-speedbar-projectile-speedbar-enable nil)
