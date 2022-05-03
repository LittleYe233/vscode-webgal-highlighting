# WebGAL Highlighting Test

## Introduction

This folder is a test of this extension. You can start a debugger or install the extension and then inspect whether the extension works well.

## Structure

The folder structure is (almost) the same as that in real time. At present all WebGAL configuration and script files are stored in `game/` folder. Though it's not necessary to set up such kind of structure now, it may be useful if this extension has a trend to become powerful or WebGAL supports more complicated syntaxes.

## Supported syntaxes

Here is a list of (almost) all syntaxes of WebGAL, where those checked are supported by the extension and can be tested via "Developer: Inspect Editor Tokens and Scopes".

- Configurations (`game/config.txt`)
  - [x] Game name (`Game_name`)
  - [x] Game key (`Game_key`)
  - [x] Image in the title screen (`Title_img`)
  - [x] Background music in the title screen (`Title_bgm`)
- Scenarios (`game/scene/*.txt`)
  - [ ] Conversations (`<Speaker>:<Sentence>;`)
    - [ ] Conversations without speakers (`<Sentence>;`)
  - [x] Black screen sentences (`intro`)
  - Backgrounds and "tachie" (full-body standing drawings of characters)
    - [x] Change (`changeBg`, `changeFigure`)
    - [ ] Transformation (`setBgTransform`)
    - [ ] Filters (`setBgFilter`)
  - [x] Mini avatars (`miniAvatar`)
  - Process controls
    - [x] Scenarios (`changeScene`, `callScene`)
    - [x] Branches (`choose`)
    - [x] Title screen (`end`)
    - [x] Labels (`jumpLabel`, `label`)
  - [x] Background music (`bgm`)
  - [x] Videos (`playVideo`)
  - Animations
    - [x] Backgrounds (`setBgAni`)
    - [x] "tachie" (`setFigAni`)
      - [ ] CSS
  - Special effects (PixiJS)
    - [x] Initialize (`pixiInit`)
    - [x] Perform (`pixiPerform`)
  - Variables **(awaiting development)**
- General
  - [x] Options (`-left`, `-right`, `-next`)
  - [x] Comments (`//`)
  - [x] Brackets (`()`)

## Acknowledgement

Most of the code of this folder is from the [instructions](https://docs.msfasr.com/guide) of WebGAL. Greatly appreciate the developers of them.