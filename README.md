# Easy Eye Yellow for VS Code

A local VS Code theme extension based on IntelliJ IDEA's archived
`EasyEyesYellow` color scheme.

The original scheme came from the old Color Themes archive:

- Archive JAR: https://raw.githubusercontent.com/dvoyni/color-themes/master/db_dump/all-color-themes.jar
- File inside the JAR: `colors/EasyEyesYellow.xml`

## Palette

The theme keeps the original editor colors as closely as VS Code allows:

| IntelliJ role | Color |
| --- | --- |
| Editor background | `#FFFFE6` |
| Text foreground | `#000000` |
| Selection background | `#DCDCDC` |
| Current line | `#F6F6F6` |
| Keywords | `#0000A0` |
| Strings | `#018A8A` |
| Numbers and escapes | `#801F91` |
| Line comments | `#38B5B5` |
| Block/doc comments | `#008040` |
| Classes | `#800000` |
| Interfaces/enums | `#18AADE` |

## Alignment Notes

The VS Code theme was checked against the archived `EasyEyesYellow.xml`
scheme. Every 6-digit color used by the original IDEA scheme is represented in
this theme, including less common values such as `#B0B0A3` for default static
methods and `#004F27` for IDEA's language-specific static method attributes.

Some IDEA color roles do not have exact VS Code equivalents because the two
editors expose different token and UI models. In those cases, this theme maps
the original role to the closest VS Code color key, TextMate scope, or semantic
token selector.

## Use Locally

From this directory:

```sh
npm run package
code --install-extension easy-eye-yellow-0.0.1.vsix
```

Then choose `Easy Eye Yellow` from VS Code's color theme picker.
