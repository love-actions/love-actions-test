# love-actions-test

## About

Github Action for auto testing sources and logics of a [LÖVE](https://love2d.org/) framework based game.

### Related actions

See related actions below:

[Love actions bare package](https://github.com/marketplace/actions/love-actions-bare-package)
[Love actions for android](https://github.com/marketplace/actions/love-actions-for-android)

## Quick example

```yaml
- name: Build bare love package
  uses: 26F-Studio/love-actions-test@main
  with:
    font-file: "./assets/fonts/proportional.otf"
    language-folder: "./assets/language"
    love-package: "./game.love"
    source-folder: "."
```

## All inputs

| Name              | Required | Default         | Description                                                  |
| :---------------- | -------- | --------------- | ------------------------------------------------------------ |
| `font-file`       | `false`  | `""`            | App main font file, would skip font coverage tests if not specified |
| `language-folder` | `false`  | `""`            | App language folder, would skip font coverage tests if not specified |
| `love-package`    | `false`  | `"./game.love"` | `.love` game package file path                               |
| `source-folder`   | `false`  | `"."`           | App source codes folder, used in grammar checks              |
