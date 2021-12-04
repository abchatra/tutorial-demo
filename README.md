## Use the tutorial

This is a microbit tutorial 
Add new tutorial as md files 

# Sample MakeCode Tutorial

This repository is an example of how to host a MakeCode tutorial on Github. This particular tutorial is for micro:bit, but this is fully supported for Arcade and Minecraft as well.

## Creating a Tutorial

To create your tutorial repository:

* Open [https://makecode.microbit.org/](https://makecode.microbit.org) (or arcade.makecode.com , minecraft.makecode.com)
* Click on **New Project**
* Give the project a descriptive name
* Click on the **Github Icon** on the bottom toolbar next to the project name and sign in if prompted
* Click **Go ahead**

This will make an empty MakeCode repository in your Github account.

## Tutorial Files

By default, the content from the README file is loaded as a tutorial. You can view it using this URL:

> [https://makecode.microbit.org/#tutorial:github:abchatra/tutorial-demo-test/turtle](https://makecode.microbit.org/#tutorial:github:abchatra/tutorial-demo-test/turtle)

The url should be formatted as follows: `https://[editor URL]/#tutorial:[github-username]/[github-repository-name]`

You can also include additional tutorials in one repository. If you add a new file, make sure it is included in the `files` list in `pxt.json`. If you add this file from the MakeCode Editor, it will be automatically updated.

The url should be formatted as follows: `https://[editor URL]/#tutorial:[github-username]/[github-repository-name]/[path-to-tutorial]`

## Custom Blocks

A repository containing a tutorial may also contain custom blocks for use in the tutorial. The `custom.ts` file here exports two functions as blocks. These blocks can then be used in any tutorial in the same repository. As with new tutorial files, make sure any new TypeScript files are added to the list in `pxt.json`.

## Custom Localization

Localized versions of the tutorial can also be added to the repository, under a `_locales` folder. This folder contains a list of sub-directories with the correctly capitalized language code (eg. zh-CN, de-DE). The localized tutorial should have the same file name as the base tutorial. To view a localized version of the tutorial, add `?lang=[language-code]` to the URL, as follows:

> [http://arcade.makecode.com?lang=zh-CN#tutorial:https://github.com/microsoft/pxt-tutorial-sample/first-tutorial](http://arcade.makecode.com?lang=zh-CN#tutorial:https://github.com/microsoft/pxt-tutorial-sample/first-tutorial)

## Creating a Release

When you update the Github repository, it make take up to 20 minutes for your changes to be reflected in the MakeCode editor, due to caching. To force an update, you will need to create a "release":

* Open [https://makecode.microbit.org/](https://makecode.microbit.org/) (or arcade.makecode.com, minecraft.makecode.com)
* Click on **Import** on the right-hand side above the row of your projects
* Select **Your Github Repo** and sign into Github if prompted
* Select the repository with your tutorial
* In the MakeCode editor, click the **Github Icon** on the bottom toolbar by the project name
* In the **Release Zone** section of the page, click **Create a Release** and select whichever release type feels most appropriate.

## License

MIT
