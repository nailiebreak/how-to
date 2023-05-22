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
  // extensions
  "git.openRepositoryInParentFolders": "never",
  "javascript.format.insertSpaceAfterConstructor": true,
  "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
  "javascript.format.semicolons": "remove",
  "javascript.preferences.quoteStyle": "single",
  "typescript.format.insertSpaceBeforeFunctionParenthesis": true,
  "typescript.format.semicolons": "remove",
  "typescript.preferences.quoteStyle": "single",
  "prettier.arrowParens": "avoid",
  "prettier.htmlWhitespaceSensitivity": "ignore",
  "prettier.jsxSingleQuote": true,
  "prettier.printWidth": 120,
  "prettier.semi": false,
  "http.proxy": "http://127.0.0.1:10800",
  "update.enableWindowsBackgroundUpdates": false,

  // text editor
  "diffEditor.diffAlgorithm": "advanced",
  "editor.codeActionsOnSave": {
    "source.organizeImports": true
  },
  "editor.codeLensFontFamily": "'Fira Code', Consolas, 'Courier New', monospace",
  "editor.copyWithSyntaxHighlighting": false,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.fontFamily": "'Fira Code', Consolas, 'Courier New', monospace",
  "editor.fontSize": 24,
  "editor.formatOnPaste": true,
  "editor.formatOnSave": true,
  "editor.minimap.enabled": false,
  "editor.tabSize": 2,
  "files.eol": "\n",
  "files.insertFinalNewline": true,
  "files.trimTrailingWhitespace": true,

  // workbench
  "breadcrumbs.enabled": false,
  "workbench.startupEditor": "none",
  "workbench.colorTheme": "One Dark Pro Darker",
  "workbench.iconTheme": "material-icon-theme",

  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
}
```
