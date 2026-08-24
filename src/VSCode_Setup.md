<div align="center">

# ⚡ VS Code Setup

_Extensions → Apps → Shortcuts → Settings — copy, paste, done._

<img src="./public/VS_Code_demo.png" width="500px" alt="VS Code Setup Preview">

</div>

---

<table align="center">
<tr>
<td valign="top" width="50%">

### 🧩 Extensions &nbsp;`Ctrl + Shift + X`

| Extensions Names              | Extensions Names          |
| ----------------------------- | ------------------------- |
| 1. Code Runner                | 7. Multiple Cursor Case   |
| 2. ES7 React/Redux/GraphQL... | 8. One Dark Pro           |
| 3. File Tree Extractor        | 9. Prettier               |
| 4. Fluent Icons               | 10. Tailwind CSS          |
| 5. Live Server                | 11. VsCode Action Buttons |
| 6. Material Icon Theme        |                           |

---

### 🖥️ Apps to Install

| Apps Names                                           | Apps Names                                                                                                   |
| ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| 1. [VS Code](https://code.visualstudio.com/download) | 5. [JetBrains Mono Font](https://github.com/niladri-1/niladri-1/raw/main/src/font/JetBrainsMono-Regular.ttf) |
| 2. [Node.js](https://nodejs.org/en/download/current) | 6. [NVM (`latest` + `v18`)](https://www.nvmnode.com/guide/download.html)                                     |
| 3. [Git](https://git-scm.com/install/windows)        | 7. [Chrome](https://www.google.com/chrome/what-you-make-of-it)                                               |
| 4. [Postman](https://git-scm.com/install/windows)    | 8. [MongoDB](https://www.mongodb.com/try/download/terraform-provider)                                        |

```bash
nvm list          # see installed version
nvm install v18   # install
nvm use v18       # switch
nvm uninstall v18 # remove
```

</td>
<td valign="top" width="50%">

### ⌨️ Shortcuts

| Shortcut                 | Action                   |
| ------------------------ | ------------------------ |
| `Ctrl + P`               | Quick file open          |
| `Ctrl + R`               | Recent workspaces        |
| `Ctrl + D`               | Select next match        |
| `Ctrl + L`               | Select current line      |
| `Ctrl + W`               | Close tab                |
| `Ctrl + B`               | Toggle sidebar           |
| `` Ctrl + ` ``           | Toggle terminal          |
| `Ctrl + Shift + K`       | Delete line              |
| `Ctrl + Shift + O`       | Go to symbol             |
| `Ctrl + Shift + [` / `]` | Fold / Unfold            |
| `Alt + ↑ / ↓`            | Move line up / down      |
| `Alt + Shift + F`        | Format document          |
| `Ctrl + Alt + ↑ / ↓`     | Add cursor above / below |

</td>
</tr>
</table>

---

<table align="center">
<tr>
<td valign="top" width="50%">

## ⚙️ Settings

`Ctrl + Shift + P` → **Open User Settings (JSON)** → select all → paste → save

<details>
<summary>Click to expand settings.json</summary>

```json
{
  "workbench.startupEditor": "none",
  "workbench.hover.delay": null,
  "workbench.editor.openSideBySideDirection": "right",
  "workbench.sideBar.location": "left",
  "workbench.tree.enableStickyScroll": true,
  "workbench.iconTheme": "material-icon-theme",
  "workbench.tree.renderIndentGuides": "none",
  "workbench.list.smoothScrolling": true,
  "workbench.tree.indent": 15,
  "workbench.editor.showTabs": "none",
  "workbench.editor.limit.value": 1,
  "workbench.editor.limit.enabled": true,
  "workbench.editor.limit.perEditorGroup": true,
  "workbench.tips.enabled": false,
  "workbench.navigationControl.enabled": false,
  "workbench.secondarySideBar.defaultVisibility": "hidden",
  "workbench.browser.showInTitleBar": false,
  "workbench.activityBar.location": "top",
  "workbench.settings.enableNaturalLanguageSearch": false,
  "workbench.editor.enablePreview": false,
  "workbench.colorTheme": "One Dark Pro Night Flat",
  "workbench.productIconTheme": "fluent-icons",
  "workbench.editor.editorActionsLocation": "hidden",
  "workbench.layoutControl.enabled": false,
  "window.menuBarVisibility": "toggle",
  "window.title": "${dirty} ${activeEditorMedium}",
  "window.newWindowDimensions": "inherit",
  "window.commandCenter": false,
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "explorer.sortOrder": "type",
  "explorer.compactFolders": false,
  "explorer.confirmPasteNative": false,
  "editor.showFoldingControls": "never",
  "editor.foldingHighlight": false,
  "editor.lineHeight": 23,
  "editor.fontSize": 14.5,
  "editor.fontFamily": "'JetBrains Mono', monospace",
  "editor.fontLigatures": true,
  "editor.cursorWidth": 3,
  "editor.cursorBlinking": "phase",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorSurroundingLines": 5,
  "editor.mouseWheelZoom": true,
  "editor.renderWhitespace": "none",
  "editor.linkedEditing": true,
  "editor.codeLens": false,
  "editor.copyWithSyntaxHighlighting": false,
  "editor.parameterHints.enabled": false,
  "editor.suggest.insertMode": "replace",
  "editor.hover.enabled": "off",
  "editor.hover.delay": 1500,
  "editor.rename.enablePreview": false,
  "editor.smoothScrolling": true,
  "editor.tabSize": 2,
  "editor.guides.indentation": false,
  "editor.wordWrap": "on",
  "editor.matchBrackets": "never",
  "editor.autoClosingDelete": "always",
  "editor.lightbulb.enabled": "off",
  "editor.guides.bracketPairs": "active",
  "editor.detectIndentation": false,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.insertSpaces": false,
  "editor.selectionHighlight": false,
  "editor.overviewRulerBorder": false,
  "editor.renderLineHighlight": "none",
  "editor.occurrencesHighlight": "off",
  "editor.hideCursorInOverviewRuler": true,
  "editor.glyphMargin": false,
  "editor.lineNumbers": "on",
  "editor.formatOnSave": true,
  "editor.suggest.showWords": false,
  "editor.snippetSuggestions": "top",
  "editor.suggest.showInlineDetails": false,
  "editor.suggest.localityBonus": true,
  "editor.accessibilitySupport": "off",
  "editor.formatOnPaste": true,
  "editor.scrollbar.horizontal": "hidden",
  "editor.scrollbar.vertical": "auto",
  "editor.scrollbar.verticalScrollbarSize": 10,
  "editor.minimap.enabled": false,
  "editor.minimap.autohide": "mouseover",
  "editor.minimap.renderCharacters": false,
  "editor.minimap.size": "fit",
  "editor.stickyScroll.enabled": false,
  "editor.suggestOnTriggerCharacters": true,
  "editor.emptySelectionClipboard": false,
  "editor.codeActionsOnSave": {
    "source.sortImports": "always",
    "source.addMissingImports": "always",
    "source.organizeImports": "always"
  },
  "diffEditor.ignoreTrimWhitespace": true,
  "diffEditor.hideUnchangedRegions.enabled": true,
  "breadcrumbs.enabled": false,
  "files.autoSave": "afterDelay",
  "files.autoSaveDelay": 1000,
  "files.trimTrailingWhitespace": true,
  "files.trimFinalNewlines": true,
  "files.eol": "\n",
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.smoothScrolling": true,
  "terminal.integrated.fontFamily": "'Source Code', 'Source Code', 'JetBrains Mono'",
  "terminal.integrated.fontWeight": "normal",
  "terminal.integrated.fontSize": 14,
  "terminal.integrated.cursorBlinking": true,
  "terminal.integrated.cursorStyleInactive": "underline",
  "terminal.integrated.stickyScroll.enabled": false,
  "terminal.integrated.initialHint": false,
  "terminal.integrated.showLinkHover": false,
  "terminal.integrated.tabs.focusMode": "singleClick",
  "code-runner.runInTerminal": true,
  "code-runner.ignoreSelection": true,
  "material-icon-theme.hidesExplorerArrows": true,
  "liveServer.settings.donotVerifyTags": true,
  "liveServer.settings.donotShowInfoMsg": true,
  "chat.disableAIFeatures": true,
  "git.autofetch": true,
  "git.openRepositoryInParentFolders": "always",
  "css.lint.unknownAtRules": "ignore",
  "css.lint.vendorPrefix": "ignore",
  "emmet.showSuggestionsAsSnippets": true,
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "typescript": "typescriptreact"
  },
  "js/ts.updateImportsOnFileMove.enabled": "always",
  "prettier.singleQuote": true,
  "prettier.printWidth": 100,
  "prettier.singleAttributePerLine": false,
  "prettier.proseWrap": "always",
  "prettier.htmlWhitespaceSensitivity": "ignore",
  "prettier.semi": true,
  "prettier.tabWidth": 2,
  "prettier.trailingComma": "all",
  "prettier.arrowParens": "always",
  "prettier.bracketSpacing": true,
  "prettier.bracketSameLine": false,
  "prettier.jsxSingleQuote": false,
  "prettier.endOfLine": "lf",
  "telemetry.telemetryLevel": "error",
  "npm.fetchOnlinePackageInfo": false,
  "search.exclude": {
    "**/node_modules": true,
    "**/dist": true,
    "**/build": true
  },
  "[snippets]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "files.associations": {
    ".prettierrc": "json",
    ".eslintrc": "json",
    ".stylelintrc": "json"
  },
  // VsCode Action Buttons
  "actionButtons": {
    "reloadButton": "$(sync) Reload",
    "defaultColor": "#9DA5B4",
    "commands": [
      {
        "name": "$(symbol-event) Vite",
        "tooltip": "Create Vite application",
        "color": "#9DA5B4",
        "command": "npm create vite@latest ./"
      },
      {
        "name": "$(package) init",
        "tooltip": "Initialize npm",
        "color": "#9DA5B4",
        "command": "npm init -y"
      },
      {
        "name": "$(server) Packages",
        "tooltip": "Install backend packages: Express, Nodemon, Mongoose, Dotenv, Cors",
        "color": "#9DA5B4",
        "command": "npm install express nodemon mongoose dotenv cors"
      },
      {
        "name": "$(play) Dev",
        "tooltip": "Run npm run dev",
        "color": "#9DA5B4",
        "command": "npm run dev"
      },
      {
        "name": "$(play) Start",
        "tooltip": "Run npm start",
        "color": "#9DA5B4",
        "command": "npm start"
      },
      {
        "name": "$(versions) Node 18",
        "tooltip": "Switch to Node.js 18",
        "color": "#9DA5B4",
        "command": "nvm use 18"
      },
      {
        "name": "$(versions) Node 24",
        "tooltip": "Switch to Node.js 24",
        "color": "#9DA5B4",
        "command": "nvm use 24"
      }
    ]
  }
}
```

</details>

</td>
<td valign="top" width="50%">

## ⚙️ Snippet Config File

<details>
<summary>Click to expand global.code-snippets</summary>

```json
{
  "CSS * Code Snippet": {
    "scope": "css,scss,sass,less,postcss",
    "prefix": "*_&_root_snippet",
    "body": [
      "* {",
      "  margin: 0;",
      "  padding: 0;",
      "  box-sizing: border-box;",
      "}",
      "",
      ":root {",
      "  /* Colors for buttons and links */",
      "  --primary-color: hsl(239, 84%, 67%); /* Main indigo color for primary actions */",
      "  --primary-hover: hsl(243, 75%, 59%); /* Hover color when mouse is over buttons */",
      "  --secondary-color: hsl(160, 84%, 39%); /* Emerald green for success alerts and icons */",
      "  --accent-color: hsl(350, 89%, 60%); /* Rose Red - alerts, CTA highlights */",
      "",
      "  /* Background colors */",
      "  --bg-primary: hsl(0, 0%, 0%); /* Pure black background for the main screen */",
      "  --bg-secondary: hsl(0, 0%, 7%); /* Very dark gray background for cards and boxes */",
      "  --bg-tertiary: hsl(0, 0%, 13%); /* Slightly lighter gray for active menu items */",
      "",
      "  /* Text colors */",
      "  --text-primary: hsl(0, 0%, 100%); /* Pure white text for main content */",
      "  --text-secondary: hsl(240, 5%, 65%); /* Soft gray text for minor details */",
      "  --text-disabled: hsl(215, 16%, 47%); /* Disabled states, placeholders */",
      "",
      "  /* Borders & Dividers */",
      "  --border-color: hsl(240, 4%, 16%); /* Border lines between sections */",
      "}",
      ""
    ]
  },
  "CSS Box Shadow": {
    "scope": "css,scss,sass,less,postcss",
    "prefix": "box_shadow_snippt",
    "body": [
      "box-shadow: ${1:inset} ${2:0}px ${3:0}px ${4:10}px ${5:0px} ${6:rgba(0, 0, 0, 0.5)};",
      "/* box-shadow: [inset] <offset-x> <offset-y> <blur-radius> <spread-radius> <color>; */"
    ]
  },
  "CSS Text Shadow": {
    "scope": "css,scss,sass,less,postcss",
    "prefix": "text_shadow_snippt",
    "body": [
      "text-shadow: ${1:0}px ${2:0}px ${3:2}px ${4:rgba(0, 0, 0, 0.5)};",
      "/* text-shadow: <offset-x> <offset-y> <blur-radius> <color>; */"
    ]
  },
  "CSS Animation Code": {
    "scope": "css,scss,sass,less,postcss",
    "prefix": "animation_snippt",
    "body": [
      "animation-name: ${1:slideIn};",
      "animation-duration: ${2:1s};",
      "animation-timing-function: ${3:ease-out};",
      "animation-delay: ${4:0.5s};",
      "animation-iteration-count: ${5:1};",
      "animation-direction: ${6:normal};",
      "animation-fill-mode: ${7:both};",
      "animation-play-state: ${8:running};",
      "}",
      "",
      "@keyframes slideIn {",
      "  from {",
      "    opacity: 0;",
      "    transform: translateY(20px);",
      "  }",
      "  to {",
      "    opacity: 1;",
      "    transform: translateY(0px);",
      "  }",
      ""
    ]
  },
  "JypeScript Jsconfig": {
    "scope": "json, jsonc",
    "prefix": "jsconfig_snippet",
    "body": [
      "{",
      "  \"compilerOptions\": {",
      "    \"target\": \"ES2020\",",
      "    \"module\": \"ESNext\",",
      "    \"moduleResolution\": \"Bundler\",",
      "    \"lib\": [\"DOM\", \"DOM.Iterable\", \"ES2020\"],",
      "    \"jsx\": \"react-jsx\",",
      "    \"strict\": true,",
      "    \"skipLibCheck\": true,",
      "    \"esModuleInterop\": true,",
      "    \"forceConsistentCasingInFileNames\": true,",
      "    \"declaration\": true,",
      "    \"declarationMap\": true,",
      "    \"sourceMap\": true,",
      "    \"isolatedModules\": true,",
      "    \"noUncheckedIndexedAccess\": true",
      "  },",
      "  \"include\": [\"src\"]",
      "}",
      ""
    ]
  },
  "Prettier RC Configuration": {
    "scope": "json, jsonc",
    "prefix": "prettier_snippet",
    "body": [
      "{",
      "  \"singleQuote\": true,",
      "  \"printWidth\": 100,",
      "  \"singleAttributePerLine\": false,",
      "  \"proseWrap\": \"always\",",
      "  \"htmlWhitespaceSensitivity\": \"ignore\",",
      "  \"semi\": true,",
      "  \"tabWidth\": 2,",
      "  \"trailingComma\": \"all\",",
      "  \"arrowParens\": \"always\",",
      "  \"bracketSpacing\": true,",
      "  \"bracketSameLine\": false,",
      "  \"jsxSingleQuote\": false,",
      "  \"endOfLine\": \"lf\"",
      "}",
      ""
    ]
  }
}
```

</details>

</td>
</tr>
</table>
