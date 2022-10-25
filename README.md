# love-actions-test

## About

Github Action for auto testing sources and logics of a [LÖVE](https://love2d.org/) framework based game.

### Related actions

See related actions below:

[Love actions bare package](https://github.com/marketplace/actions/love-actions-bare-package)

[Love actions for android](https://github.com/marketplace/actions/love-actions-for-android)

[Love actions for iOS](https://github.com/marketplace/actions/love-actions-for-ios)

[Love actions for Linux](https://github.com/marketplace/actions/love-actions-for-linux)

[Love actions for macOS portable](https://github.com/marketplace/actions/love-actions-for-macos-portable)

[Love actions for macOS AppStore](https://github.com/marketplace/actions/love-actions-for-macos-appstore)

[Love actions for Windows](https://github.com/marketplace/actions/love-actions-for-windows)

## Quick example

```yaml
- name: Build bare love package
  uses: love-action/love-actions-test@v1
  with:
    font-file: "./assets/fonts/proportional.otf"
    language-folder: "./assets/language"
    love-package: "./game.love"
    source-folder: "."
    strict: "true"
```

## All inputs

| Name                | Required  | Default           | Description                                                          |
| :------------------ | --------- | ----------------- | -------------------------------------------------------------------- |
| `font-file`       | `false` | `""`            | App main font file. Would skip font coverage tests if not specified  |
| `language-folder` | `false` | `""`            | App language folder. Would skip font coverage tests if not specified |
| `love-package`    | `false` | `"./game.love"` | `.love` game package file path                                     |
| `source-folder`   | `false` | `"."`           | App source codes folder. Used in grammar checks                      |
| `strict`          | `false` | `"false"`       | Strict mode. Fail the tests if font coverage is not 100%             |
