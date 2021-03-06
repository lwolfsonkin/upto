[![Build Status][travis-badge]][travis-link]
[![Slack Room][slack-badge]][slack-link]

# upto

Gets you to a parent folder, heavily inspired by the plugin [upto](https://github.com/driv/upto) made by [driv](https://github.com/driv).

## Install

With [fisherman]

```
fisher upto
```

## Usage

Inside */home/username/Projects/project_a/src/Core*

```fish
$ upto Projects
$ pwd
/home/username/Projects
```

It works on directories with non ASCII characters if the charset used is UTF-8. 

Inside */home/weiß/projekten/src/Core*

```fish
$ upto weiß
$ pwd
/home/weiß
```

You can use it inside directories with spaces too. 

Inside */home/User/My Documents/xls/2016/essays*

```fish
$ upto "My Documents"
$ pwd
/home/User/My Documents
```

[travis-link]: https://travis-ci.org/fisherman/upto
[travis-badge]: https://img.shields.io/travis/fisherman/upto.svg
[slack-link]: https://fisherman-wharf.herokuapp.com
[slack-badge]: https://fisherman-wharf.herokuapp.com/badge.svg
[fisherman]: https://github.com/fisherman/fisherman
