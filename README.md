# WebGAL Support for Visual Studio Code

**GitHub:** <https://github.com/LittleYe233/vscode-webgal-highlighting>

**NPM:** <https://www.npmjs.com/package/vscode-webgal-highlighting>

![npm](https://img.shields.io/npm/v/vscode-webgal-highlighting?style=flat-square) [![GitHub license](https://img.shields.io/github/license/LittleYe233/vscode-webgal-highlighting?style=flat-square)](https://github.com/LittleYe233/vscode-webgal-highlighting/blob/main/LICENSE) [![GitHub issues](https://img.shields.io/github/issues/LittleYe233/vscode-webgal-highlighting?style=flat-square)](https://github.com/LittleYe233/vscode-webgal-highlighting/issues)

This package is a Visual Studio Code extension to provide language support for [MakinoharaShoko/WebGAL](https://github.com/MakinoharaShoko/WebGAL/).

WebGAL is a brand new visual novel engine based on Web and is still under development and code refactoring, its stable releases published.

Now this extension is still being tested and waiting for more stable syntaxes supported by WebGAL.

This extension will complete more complicated language support like semantic highlighting in the future.

## Features

- Syntax highlighting
  - Keywords (`changeBG`, `if`, `setVar`, etc.)
  - Comments

**Note:** This extension doesn't specify any preferred file type to provide language support, for the extension of all WebGAL scripts is ".txt". You can specify the viewing language to "WebGAL Script (webgal)" for the scripts at the right bottom corner of Visual Studio Code.

## Requirements

### Users

There is no more requirement for Visual Studio Code user. Just install the extension in the marketplace and enjoy it.

### Developers

All requirements on dependencies are written in `package.json`. After cloning the repository, execute `npm install` in it via your preferred terminal.

<!-- ## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

* `myExtension.enable`: enable/disable this extension
* `myExtension.thing`: set to `blah` to do something -->

<!-- ## Known Issues

Calling out known issues can help limit users opening duplicate issues against your extension. -->

## Release Notes

Please check [CHANGELOG.md](/CHANGELOG.md).