# Basic Editing

## Multiple Selections

- add secondary cursors with **`Alt+Click`**.
- insert cursors below or above with **`Ctrl+Alt+Down/Up`**.
- select the word at the cursor or the next occurrence of the current selection with **`Ctrl+D`**.
- add a selection at each occurrence of the current selected text with **`Ctrl+Shift+L`**.

## Shrink/Expand Selection

- quickly shrink or expand the current selection with **`Shift+Alt+Left/Right`**.

## Formatting

- format the entire active file with **`Shift+Alt+F`**.
- format the selected text with **`Ctrl+K Ctrl+F`**.
- you can also trigger formatting based on user gestures such as typing, saving or pasting. These are off by defult but you can enable these behaviors through the following settings:

  - `editor.formatOnType` - format the line after typing.
  - `editor.formatOnSave` - format a file on save.
  - `editor.formatOnPaste` - format the pasted content.

## Folding

- fold/unfold the innermost uncollapsed/collapsed region at the cursor with **`Ctrl+Shift+[/]`** or **`Ctrl+K Ctrl+L`**.
- fold/unfold recursively the innermost uncollapsed/collapsed region at the cursor and all regions inside that region with **`Ctrl+K Ctrl+[/]`**.
- fold/unfold all regions in the editor with **`Ctrl+K Ctrk+0/J`**.
- fold all regions that start with a block comment token with **`Ctrl+K Ctrl+/`**.

# Code Navigation

## Quick File Navigation

- open any file by its name with **`Ctrl+P`**.
- navigate symbols inside a file with **`Ctrl+Shift+O`**.
- go to a symbol across files with **`Ctrl+T`**.
- hold **`Ctrl`** and press **`Tab`** to view a list of all files open in an editor group.
- you can go to the definition of a symbol with **`F12`**.
- you can go to the definition of a symbol with **`Ctrl+Click`** or open the definition to the side with **`Ctrl+Alt+Click`**.
- you can preview of the declaration of a symbol by hovering it with pressing **`Ctrl`**.
- you can go to the implementation of a symbol by **`Ctrl+F12`**.
- go to reference (via **`Shift+F12`**) or peek definition (via **`Alt+F12`**).
- jump to the matching bracket with **`Ctrl+Shift+\`**.

# Integrated Terminal

## Run Selected Text

- select text in an editor and run the command **_Terminal: Run Selected Text in Active Terminal_** via the **Command Palette**.

# **Current Visual Studio Code Settings**

```json
{
  // Text Editor
  "editor.copyWithSyntaxHighlighting": false,
  "editor.cursorBlinking": "expand",
  "editor.cursorStyle": "line-thin",
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.detectIndentation": false,
  "editor.fontFamily": "'Cascadia Code', 'Fira Code', 'DejaVu Sans Mono', Consolas",
  "editor.fontSize": 20,
  "editor.formatOnPaste": true,
  "editor.formatOnSave": true,
  "editor.minimap.enabled": false,
  "editor.scrollBeyondLastLine": false,
  "editor.tabSize": 2,
  "files.enableTrash": false,
  "files.insertFinalNewline": true,
  "files.trimTrailingWhitespace": true,
  // Workbench
  "workbench.colorCustomizations": {
    "activityBarBadge.background": "#FF7042",
    "activityBar.activeBorder": "#FF7042",
    "list.activeSelectionForeground": "#FF7042",
    "list.inactiveSelectionForeground": "#FF7042",
    "list.highlightForeground": "#FF7042",
    "scrollbarSlider.activeBackground": "#FF704250",
    "editorSuggestWidget.highlightForeground": "#FF7042",
    "textLink.foreground": "#FF7042",
    "progressBar.background": "#FF7042",
    "pickerGroup.foreground": "#FF7042",
    "tab.activeBorder": "#FF7042",
    "notificationLink.foreground": "#FF7042",
    "editorWidget.resizeBorder": "#FF7042",
    "editorWidget.border": "#FF7042",
    "settings.modifiedItemIndicator": "#FF7042",
    "settings.headerForeground": "#FF7042",
    "panelTitle.activeBorder": "#FF7042",
    "breadcrumb.activeSelectionForeground": "#FF7042",
    "menu.selectionForeground": "#FF7042",
    "menubar.selectionForeground": "#FF7042",
    "editor.findMatchBorder": "#FF7042",
    "selection.background": "#FF704240"
  },
  "workbench.colorTheme": "Material Theme Palenight High Contrast",
  "workbench.iconTheme": "vscode-icons",
  "workbench.startupEditor": "none",
  "breadcrumbs.enabled": false,
  // Window
  "window.zoomLevel": 0,
  // Features
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "explorer.sortOrder": "type",
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.fontFamily": "'Cascadia Code'",
  "terminal.integrated.fontSize": 18,
  // Extensions
  "git.enableSmartCommit": true,
  "git.autoRepositoryDetection": false,
  "materialTheme.accent": "Orange",
  "javascript.format.insertSpaceAfterConstructor": true,
  "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
  "javascript.format.semicolons": "remove",
  "javascript.preferences.quoteStyle": "single",
  "javascript.updateImportsOnFileMove.enabled": "never",
  "typescript.format.insertSpaceBeforeFunctionParenthesis": true,
  "typescript.format.semicolons": "remove",
  "typescript.preferences.quoteStyle": "single"
}
```
