# Git Smart Checkout

This is a dumb little library I made because I don't like using autocomplete to checkout a branch.

This will print out a prompt showing the local branches in your current repo and allow you to check one of these out based on the number allocated to it:

```
Checkout a branch:

  1: bug_fix/different_sized_tables
  2: develop
  3: fix_flaky_amount_specs
  4: nullable_factory_fields

Type the number of the branch you want to checkout: 3

Switched to branch 'fix_flaky_amount_specs'
```

## Setup

To call this library from the command line, you have to make the ruby file available in your $PATH.

You'll want to clone this repo somewhere, then symlink the `git_smart_checkout.rb` file somewhere on your $PATH. EG:

```
chmod +x git_smart_checkout.rb
ln -s `pwd`/git_smart_checkout.rb ~/bin/git_smart_checkout
```

## TODO

- Support checking out remote branches
