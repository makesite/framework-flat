makesite framework-flat
======================

NOTE: UNTIL FURTHER NOTICE, THIS REPO IS *NOT* USABLE AS-IS.
YOU WOULD HAVE TO EDIT SOME FILES TO MAKE IT WORK. THIS IS
A WORK IN PROGRESS AND IS A SUBJECT TO CHANGE.

Simplistic layout for makesite framework.

As we favor configuration over convention, this is only one of many
possible uses of the (very) modular components. 

For one possible configuration, a very simplistic one, you could
use this repo.

An alternative convention is layout-flat, which is in it's own repo.

Usage
-----

```
git clone https://github.com/makesite/framework-flat.git
cd framework-flat
make init
```

If you wish to create your layout using symlinks, use

```
make layout-dev
```

For hard-copying the files instead of using symlinks, use

```
make layout-dist
```

Finally, to prepare a stand-alone .tar.gz suitable for git-less
distribution, run:

```
make dist
```

Layout
------

```
layout
├── design
├── controllers
├── models
├── files
├── config.php
├── config.dev.php
├── db.conf.php
├── install.php
└── index.php
```

Getting out of the webroot
--------------------------

Is definitly possible, but you would have to re-arrange some files
and adjust the APP_DIR and CORE_DIR constants in `config.php`.

Such a layout would be a subject for a different repository in the
future.
