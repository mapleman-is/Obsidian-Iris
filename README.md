# Obsidian Iris

### Version 1.9.9 - (2.0.0 PreRelease source)

Features Supported:

- Nested To Do items.
- Stronger file verification.
- Weekly Note rollover.

Iris is a tool for rolling over your previous day's unfinished tasks. This is based on, but not a fork of [this](https://github.com/shichongrui/obsidian-rollover-daily-todos), and is designed to work with [this plugin](https://github.com/liamcain/obsidian-calendar-plugin) for managing Daily Notes and Calendar items. 

![](https://github.com/OliverAndrews/Obsidian-Iris/blob/master/docs/images/Vault%20-%20Obsidian%20v0.10.6%202021-01-10%2016-00-03.gif)

### To Install
[Click here to download latest Iris.zip](https://github.com/OliverAndrews/Obsidian-Iris/releases/tag/1.0).

Here you should only select Iris.zip, the source files are not needed unless you want to make code changes. 

Make a folder inside Vault/.obsidian/plugins called Iris. Put the contents of Iris.zip into that folder.

Once you have installed, and set it up, close Obsidian and then reopen the program to make it work.

This plugin requires you to have a daily notes system set up using [this plugin](https://github.com/liamcain/obsidian-calendar-plugin). To create a new daily note select the calendar day that you would like to create a note for. Using the sidebar's Daily Notes button will not cause notes to roll over.

### Filenames

Iris uses the filename of your daily note as a way to determine which other note's TO DO list it will import. Because of this, the title has to be clearly formatted and look like this: `Sunday Jan 03, 2021`. This only affects filenames. Headings and other anchors are unaffected. Anyone who's coming from [obsidian-rollover-daily-todos](https://github.com/shichongrui/obsidian-rollover-daily-todos) doesn't have to make any changes and Iris is fully compatible with this plugin.

### Setting Up

![Settings Window](https://i.imgur.com/9NCsLHy.png)

**To Do** heading lets you set what anchor you have your TO DO list in. Anything in that anchor's section which starts with `- [ ]` will be imported if they are not marked as complete. 

**Daily Notes Directory** allows you to specify where your Daily Notes are kept. Anything in that directory must be formatted with the correct filename, mentioned above.

### Notes to Developers

If you would like to build from source, you can clone this directory, and run `npm install` within the repository. To run the TypeScript compiler in watch mode, run `npm run dev`. If you would like to build the documentation, run `npm run doc`. NOTE: This is developers documentation on code and won't tell you how Iris works. Once you're done, to build for production, use `npm run build-prod`. To *just* build the main.ts file, use `npm run build`. Once you build, move build folder to plugins directory.

### Bug Reports and Feature Requests

If you detect a bug in Iris, please open a new issue on this project. You may also open feature requests with issues, however implementation of feature requests is not guaranteed.
