# y2s19-editor-configs
This repo outlines instructions for configuring editor plugins for student laptops.  This is a living repository-- in the future, we may add more configuration settings.

TODO: write scripts to automate this process

## Prettier
[Prettier](https://prettier.io) is a code formatting tool, primarily used for front-end web development. We'll be using Prettier to automatically format JavaScript, HTML, and CSS files whenever a file is saved.

For all editors:
Assuming [npm](https://www.npmjs.com/get-npm) is already installed, run `npm install -g prettier` on the command line

### VSCode
1. Press `Ctrl/⌘ + P` to open the command palette, paste in `ext install esbenp.prettier-vscode`, and press enter to install the plugin. Reload the editor (`Ctrl/⌘ + R`)
2. Press `Ctrl/⌘ + ,` to open user settings, and press the curly braces button in the top right corner to manually edit user settings. Replace (or merge, if settings already exist) the following JSON into the `settings.json` file. Then, save the file.
```json
{
  "[javascript]": {
    "editor.formatOnSave": true
  },
  "[json]": {
    "editor.formatOnSave": true
  },
  "[html]": {
    "editor.formatOnSave": true
  },
  "[css]": {
    "editor.formatOnSave": true
  }
}
```

TODO:

Atom

Sublime3

WebStorm/Pycharm
