# My personal Zed settings

Settings and keymap files written for Zed to my own liking.

## Preview

![Screenshot](_assets/screenshot.png)

Screenshot taken at 12/14/2025

## Settings file

[File](settings.json) that changes Zed visually and how it behaves.

### AI & Privacy

- Disables AI
- Disables Telemetry

### Window & Layout

- Hides sign-in button on title bar & navigation history buttons on tab bar
- Shows file icons on tabs

### Theme

- [One Dark - Darkened](https://github.com/pavles6/one-dark-darkened) as dark theme
- [Catppuccin Mocha](https://github.com/catppuccin/zed-icons) as icon theme

### Editor

- Uses [Iosevka Nerd Font](https://nerdfonts.com/font-downloads#:~:text=Iosevka) as editor font
- Sets the editor font size to `13`
- Disables final newline and formatting on save
- Forces the use of tabs instead of spaces for indentation
- Sets the indentation size to `4`

### Programming Languages

Python:
- Ensures final newline on save
- Uses `pylsp` as LSP, disables `basedpyright` and `ruff`

### Language Servers

`pylsp` - Python LSP:
- Ignores some `pycodestyle` rules:

| Code | Description                       |
| ---: | --------------------------------- |
| E302 | Expected 2 blank lines, found 0-1 |
| E303 | Too many blank lines (3+)         |
| E501 | Line too long (n > 79 characters) |
| W191 | Indentation contains tabs         |
| W293 | Blank line contains whitespace    |

- Disables automatic creation of `.ropeproject` directory
- Sets the root project `.venv` directory as the used virtual environment for code completion

## Keymap file

[File](keymap.json) that adds shortcuts to some actions.

| Context    | Binding        | Action                   |
| ---------- | -------------- | ------------------------ |
| \<global\> | `CTRL-O`       | Open files               |
| \<global\> | `CTRL-Shift-O` | Open folder              |
| \<global\> | `CTRL-'`       | Toggle terminal          |
| Editor     | `CTRL-M`       | Toggle language selector |
