# WebGAL Support for Visual Studio Code

Available languages: [简体中文](README.zh-cn.md) / [English](README.md)

**GitHub:** <https://github.com/LittleYe233/vscode-webgal-highlighting>

**NPM:** <https://www.npmjs.com/package/vscode-webgal-highlighting>

![npm](https://img.shields.io/npm/v/vscode-webgal-highlighting?style=flat-square) [![GitHub license](https://img.shields.io/github/license/LittleYe233/vscode-webgal-highlighting?style=flat-square)](https://github.com/LittleYe233/vscode-webgal-highlighting/blob/main/LICENSE) [![GitHub issues](https://img.shields.io/github/issues/LittleYe233/vscode-webgal-highlighting?style=flat-square)](https://github.com/LittleYe233/vscode-webgal-highlighting/issues)

This package is a Visual Studio Code extension to provide language support for [MakinoharaShoko/WebGAL](https://github.com/MakinoharaShoko/WebGAL/).

WebGAL is a brand new visual novel engine based on Web and is still under development and code refactoring with its stable releases published.

Now this extension is still being tested and waiting for more stable syntaxes supported by WebGAL.

We will keep trying to make this extension provide more support for WebGAL in the future, including more complicated language support (semantic highlighting).

## Features

- Syntax highlighting
  - Keywords (`changeBG`, `if`, `setVar`, etc.)
  - Comments

**Note:** This extension doesn't specify any preferred file type to provide language support, for the extension of all WebGAL scripts is ".txt". You can specify the viewing language to "WebGAL Script (webgal)" for the scripts at the right bottom corner of Visual Studio Code.

## Usage

### Normal users

There is no more requirement for normal users. Just install the extension in the marketplace and enjoy it.

### Developers

All requirements on dependencies are written in `package.json`. After cloning the repository, execute `npm install` in it via your preferred terminal.

#### Develop with YAML

VS Code uses JSON files (`*.tmLanguage.json`) to highlight code, but it's sometimes a bit annoying to write these highlighting rules in JSON format. So you can write them into YAML files first, and then convert them to JSON files.

`package.json` just provides an option to easily convert YAML to JSON - `js-yaml`. To use it, first install it globally via `npm install -g js-yaml`. After installing it and writing some rules in `syntaxes/webgal.tmLanguage.yml`, execute `js-yaml syntaxes/webgal.tmLanguage.yml > syntaxes/webgal.tmLanguage.json` to apply your changes.

Of course, don't worry to directly commit your changes on JSON files - we will merge these changes and convert them to YAML later.

### Test locally

If you want to test this extension locally, open a new VS Code window in the repository folder and press `F5` to start a debugger. It will automatically load this extension and you can have a try just like normal users.

Additionally, you can choose "Developer: Inspect Editor Tokens and Scopes" from the command palette (launch it via `Ctrl`+`Shift`+`P`) to get a deeper insight into how the extension works and whether it labels all the tokens and scopes correctly or not.

<!-- ## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

* `myExtension.enable`: enable/disable this extension
* `myExtension.thing`: set to `blah` to do something -->

<!-- ## Known Issues

Calling out known issues can help limit users opening duplicate issues against your extension. -->

## Contribute

Everyone is welcome to create issues and pull requests here.

There are only few suggestions for developers who create PRs:

- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
  
  It's better to commit your changes in favor of it. More specifically,
  - please add a `<type>` like `feat`, `chore`, `build`, `revert` for your commits;
  - non-English `<description>` and `[optional body]` of a commit can be accepted;
  - you can set up [husky](https://typicode.github.io/husky/#/) to lint your commits;
  - if your commits will close any issue or PR, please take advantage of `[optional footer(s)]` like `Close #xx` and `PR Close #xx` (accepted as long as GitHub supports it).
- Scope naming

  It's better to choose appropriate names for your scopes. [TextMate 1.x Manual](https://macromates.com/manual/en/language_grammars) is mentioned in the official documentation of VS Code language extension, which includes a detailed list of conventional scope names. Also you can have a look at the built-in language files in VS Code, i.e. `json.tmLanguage.json`.

- Branches

  The upstream branch of your pull requests should be `main`, not `dev`. There is an [issue](https://github.com/LittleYe233/vscode-webgal-highlighting/issues/3) written in Chinese explaining why.

## Release Notes

Please check [CHANGELOG.md](/CHANGELOG.md).