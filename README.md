# cakephp-plugin-skel

A skeleton repo for CakePHP plugins

## Idea & Purpose

The idea behind this repository is quite simple:
Every time you create a CakePHP plugin, you have to setup the folder structure and various auxiliary files, such as ``composer.json`` and ``.travis.yml``.

This repository tries to keep you [DRY](http://en.wikipedia.org/wiki/Don%27t_repeat_yourself) by having setup everything - and most likely much more - you may need to get started writing your own plugin.
Instead of **adding** common files and folders to your plugin folder, you can **remove** unneeded files and folders from it.

## How To Use

1. Download the repository as Zip file.
2. Extract it to ``/path/to/your/cake/install/folder/app/[YourPluginName]``
3. Optionally generate the plugin AppController and AppModel by executing
`` shell
cake bake plugin [YourPluginName]
``
4. Integrate your new plugin into your own VCS (See "How To Publish Your Plugin")
5. Delete everything you don't need
6. Start working on your own plugin code by following the
[plugin section in the CakePHP book](http://book.cakephp.org/2.0/en/plugins.html#creating-your-own-plugins)

## How To Publish Your Plugin

Asuming you are going to publish your plugin on GitHub, you should:

- Create a public GitHub repo named ``your_username/cakephp-[your_plugin_name]``
- Decide whether to use the GitHub Issues
- Decide whether to use the GitHub Wiki
- Upload your code to GitHub
- Adjust the [composer.json](composer.json) by updating the following keys:
  - ``name``
  - ``description``
  - ``keywords``
  - ``homepage``
  - ``authors`, replace the "Lead Developer"
  - ``support``
  - ``require``, if your plugin depends on vendor libraries
  - ``require``, if your plugin depends on vendor libraries for development
  - ``extra/installer-name``, with your plugin name in CamelCase
- Replace [README.md](README.md) by [PLUGIN_README.md](PLUGIN_README.md)
- Adjust [CONTRIBUTING.md](CONTRIBUTING.md)
- Adjust the [.travis.yml](.travis.yml) by updating the following:
  - Replace ``PluginSkeleton`` by ``[YourPluginName]``
  - See [FriendsOfcake/Travis](https://github.com/FriendsOfCake/travis) for further options
- Consult the [CakePHP book](http://book.cakephp.org/2.0/en/plugins.html#publish-your-plugin) for further steps
