# WebGAL Highlighting Test

## Introduction

This folder is a test of this extension. You can start a debugger or install the extension and then inspect whether the extension works well.

## Structure

The folder structure is (almost) the same as that in real time. At present all WebGAL configuration and script files are stored in `game/` folder. Though it's not necessary to set up such kind of structure now, it may be useful if this extension has a trend to become powerful or WebGAL supports more complicated syntaxes.

## Supported syntaxes

Here is a list of (almost) all syntaxes of WebGAL, where those checked are supported by the extension and can be tested via "Developer: Inspect Editor Tokens and Scopes".

- Configurations (`game/config.txt`)
  - [ ] Game name (`Game_name`)
  - [ ] Game key (`Game_key`)
  - [ ] Image in the title screen (`Title_img`)
  - [ ] Background music in the title screen (`Title_bgm`)
- Scenarios (`game/scene/*.txt`)
  - [ ] Conversations (`<Speaker>:<Sentence>;`)
    - [ ] Conversations without speakers (`<Sentence>;`)
  - [ ] Black screen sentences (`intro`)
  - Backgrounds and "tachie" (full-body standing drawings of characters)
    - [ ] Change (`changeBg`, `changeFigure`)
    - [ ] Transformation (`setBgTransform`)
    - [ ] Filters (`setBgFilter`)
  - [ ] Mini avatars (`miniAvatar`)
  - Process controls
    - [ ] Scenarios (`changeScene`, `callScene`)
    - [ ] Branches (`choose`)
    - [ ] Title screen (`end`)
    - [ ] Labels (`jumpLabel`, `label`)
  - [ ] Background music (`bgm`)
  - [ ] Videos (`playVideo`)
  - Animations
    - [ ] Backgrounds (`setBgAni`)
    - [ ] "tachie" (`setFigAni`)
      - [ ] CSS
  - Special effects (PixiJS)
    - [ ] Initialize (`pixiInit`)
    - [ ] Perform (`pixiPerform`)
  - Variables **(awaiting development)**
- General
  - [ ] Options (`-left`, `-right`, `-next`)
  - [ ] Comments (`//`)

## Acknowledgement

Most of the code of this folder is from the [instructions](https://docs.msfasr.com/guide) of WebGAL. Greatly appreciate the developers of them.