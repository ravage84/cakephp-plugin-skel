# cakephp-plugin-skel

A skeleton repo for CakePHP plugins

## Idea & Purpose

The idea behind this repository is quite simple:
Every time you create a CakePHP plugin, you have to setup the folder structure and various auxiliary files, such as ``composer.json`` and ``.travis.yml``.

This repository tries to keep you [DRY](http://en.wikipedia.org/wiki/Don%27t_repeat_yourself) by having setup everything - and most likely much more - you may need to get started writing your own plugin.
Instead of **adding** common files and folders to your plugin folder, you can **remove** unneeded files and folders from it.

## How To Use

1. Download the repository as Zip file.
2. Extract it
3. Delete everything you don't need
4. Integrate it into your own VCS
5. Start working on your own plugin code

## How To Publish Your Plugin

1. Adjust the [composer.json](composer.json)
2. Adjust the [.travis.yml](.travis.yml)
