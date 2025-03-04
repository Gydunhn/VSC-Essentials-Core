# VSC Essentials Core - Pack for Developers

[![Badge for version for Visual Studio Code extension](https://flat.badgen.net/vs-marketplace/v/Gydunhn.vsc-essentials-core?icon=visualstudio&color=blue)](https://marketplace.visualstudio.com/items?itemName=Gydunhn.vsc-essentials-core) [![Installs](https://flat.badgen.net/vs-marketplace/i/Gydunhn.vsc-essentials-core?color=blue)](https://marketplace.visualstudio.com/items?itemName=Gydunhn.vsc-essentials-core) [![Downloads](https://flat.badgen.net/vs-marketplace/d/Gydunhn.vsc-essentials-core?color=blue)](https://marketplace.visualstudio.com/items?itemName=Gydunhn.vsc-essentials-core) [![Rating](https://flat.badgen.net/vs-marketplace/rating/Gydunhn.vsc-essentials-core?color=blue)](https://marketplace.visualstudio.com/items?itemName=Gydunhn.vsc-essentials-core)

This extension pack for Visual Studio Code adds extensions that are convenient and useful for any development (regardless of language). I reserve the right to update the content of the extension pack at my own discretion.

This **Detailed** version of the extension pack is for a series of very specific projects in which I am currently involved; projects with multiple repositories that share the same stack of technologies transversally.

![Preview](https://firebasestorage.googleapis.com/v0/b/vsc-essentials.appspot.com/o/VSC-Essentials-Core%2FVSC-Essentials-Core-Preview.png?alt=media&token=2a85a17f-bf06-4d68-8b6a-cee289451515)

## Reasons

The "Original & Complete" version of [VSC Essentials] extension pack was made to automate and standardize the setup phase of the development environment for Visual Studio Code, to have the same set of extensions, use the same id settings and file format everyone works on together.

See the [CHANGELOG](CHANGELOG.md) for the latest changes

## **settings.json**

It is imperative that the settings be added to settings.json, inside the ".vscode" folder, and that this file be inside Git version control for this extension pack to work correctly.

``` json
{
    /**
     * Core Basic VSC Essentials Config
     */
    "extensions.ignoreRecommendations": true,
    "editor.tabCompletion": "on",
    "editor.showDeprecated": true,
    "editor.rulers": [
        80
    ],
    "editor.guides.bracketPairs": "active",
    "editor.bracketPairColorization.independentColorPoolPerBracketType": true,
    "workbench.tree.expandMode": "singleClick",
    "workbench.tree.renderIndentGuides": "always",
    "workbench.tree.indent": 6,
    "editor.formatOnType": false,
    "editor.formatOnSave": true,
    "editor.formatOnPaste": true,
    "[markdown]": {
        "editor.defaultFormatter": "yzhang.markdown-all-in-one"
    },
    "[json]": {
        "editor.defaultFormatter": "vscode.json-language-features"
    },
    "[jsonc]": {
        "editor.defaultFormatter": "vscode.json-language-features"
    },
    "[xml]": {
        "editor.defaultFormatter": "DotJoshJohnson.xml"
    },
    "[javascript]": {
        "editor.defaultFormatter": "vscode.typescript-language-features"
    },
    "[typescript]": {
        "editor.defaultFormatter": "vscode.typescript-language-features"
    },
    "[css]": {
        "editor.defaultFormatter": "vscode.css-language-features"
    },
    "[less]": {
        "editor.defaultFormatter": "vscode.css-language-features"
    },
    "[scss]": {
        "editor.defaultFormatter": "vscode.css-language-features"
    },
    "[html]": {
        "editor.defaultFormatter": "vscode.html-language-features"
    },
    "javascript.format.enable": true,
    "javascript.format.semicolons": "insert",
    "javascript.preferences.quoteStyle": "single",
    "typescript.format.enable": true,
    "typescript.format.semicolons": "insert",
    "typescript.preferences.quoteStyle": "single",
    "css.hover.documentation": true,
    "css.lint.important": "warning",
    "css.lint.importStatement": "warning",
    "less.hover.documentation": true,
    "less.lint.important": "warning",
    "less.lint.importStatement": "warning",
    "scss.hover.documentation": true,
    "scss.lint.important": "warning",
    "scss.lint.importStatement": "warning",
    "html.hover.documentation": true,
    "markdownlint.config": {
        "default": true,
        "MD001": false,
        "MD010": false,
        "MD024": false,
        "MD025": false
    },
    /**
     * * Core Detailed VSC Essentials Config
     */
    "todo-tree.tree.showCountsInTree": true,
    "todo-tree.general.statusBar": "top three",
    "todo-tree.general.showIconsInsteadOfTagsInStatusBar": true,
    "todo-tree.general.tags": [
        "TODO",
        "FIXME",
        "FIXIT",
        "FIX",
        "BUG"
    ],
    "todo-tree.general.tagGroups": {
        "FIXME": [
            "FIXME",
            "FIXIT",
            "FIX",
            "BUG",
        ]
    },
    "todo-tree.highlights.customHighlight": {
        "TODO": {
            "gutterIcon": true,
            "icon": "tasklist",
            "iconColour": "#FF8C00",
            "type": "tag",
            "background": "#CF7200",
            "foreground": "#FFFFFF",
            "fontWeight": "bold"
        },
        "FIXME": {
            "gutterIcon": true,
            "icon": "tools",
            "iconColour": "#00FF00",
            "type": "tag",
            "background": "#008000",
            "foreground": "#FFFF00",
            "fontWeight": "bold"
        }
    },
    "better-comments.multilineComments": true,
    "better-comments.tags": [
        {
            "tag": "!",
            "color": "#FF2D00",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": true,
            "italic": false
        },
        {
            "tag": "?",
            "color": "#3498DB",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "//",
            "color": "#474747",
            "strikethrough": true,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "todo",
            "color": "#FF8C00",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "fixme",
            "color": "#008000",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "fixit",
            "color": "#008000",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "fix",
            "color": "#008000",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "bug",
            "color": "#008000",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": false,
            "italic": false
        },
        {
            "tag": "*",
            "color": "#98C379",
            "strikethrough": false,
            "underline": false,
            "backgroundColor": "transparent",
            "bold": true,
            "italic": false
        }
    ]
}

```

## Note

This extension pack was made from their original [VSC Essentials], which you can find [here].
[This extension] can be found at [open-vsx.org] as well.

## Included

This **Detailed** Core extension pack includes the following extensions:

| Extension               | Stats                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Markdown All in One     | [![Badge for version for Visual Studio Code extension](https://flat.badgen.net/vs-marketplace/v/yzhang.markdown-all-in-one?icon=visualstudio&color=blue)](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) [![Installs](https://flat.badgen.net/vs-marketplace/i/yzhang.markdown-all-in-one?color=blue)](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) [![Rating](https://flat.badgen.net/vs-marketplace/rating/yzhang.markdown-all-in-one?color=blue)](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)                                                                                     |
| markdownlint            | [![Badge for version for Visual Studio Code extension](https://flat.badgen.net/vs-marketplace/v/DavidAnson.vscode-markdownlint?icon=visualstudio&color=blue)](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) [![Installs](https://flat.badgen.net/vs-marketplace/i/DavidAnson.vscode-markdownlint?color=blue)](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) [![Rating](https://flat.badgen.net/vs-marketplace/rating/DavidAnson.vscode-markdownlint?color=blue)](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)                                                             |
| XML Tools               | [![Badge for version for Visual Studio Code extension](https://flat.badgen.net/vs-marketplace/v/DotJoshJohnson.xml?icon=visualstudio&color=blue)](https://marketplace.visualstudio.com/items?itemName=DotJoshJohnson.xml) [![Installs](https://flat.badgen.net/vs-marketplace/i/DotJoshJohnson.xml?color=blue)](https://marketplace.visualstudio.com/items?itemName=DotJoshJohnson.xml) [![Rating](https://flat.badgen.net/vs-marketplace/rating/DotJoshJohnson.xml?color=blue)](https://marketplace.visualstudio.com/items?itemName=DotJoshJohnson.xml)                                                                                                                                     |
| Todo Tree               | [![Badge for version for Visual Studio Code extension](https://flat.badgen.net/vs-marketplace/v/Gruntfuggly.todo-tree?icon=visualstudio&color=blue)](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree) [![Installs](https://flat.badgen.net/vs-marketplace/i/Gruntfuggly.todo-tree?color=blue)](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree) [![Rating](https://flat.badgen.net/vs-marketplace/rating/Gruntfuggly.todo-tree?color=blue)](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)                                                                                                                   |
| Git Graph               | [![Badge for version for Visual Studio Code extension](https://flat.badgen.net/vs-marketplace/v/mhutchie.git-graph?icon=visualstudio&color=blue)](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph) [![Installs](https://flat.badgen.net/vs-marketplace/i/mhutchie.git-graph?color=blue)](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph) [![Rating](https://flat.badgen.net/vs-marketplace/rating/mhutchie.git-graph?color=blue)](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)                                                                                                                                     |
| Terminal in Status Bar  | [![Badge for version for Visual Studio Code extension](https://flat.badgen.net/vs-marketplace/v/flyfly6.terminal-in-status-bar?icon=visualstudio&color=blue)](https://marketplace.visualstudio.com/items?itemName=flyfly6.terminal-in-status-bar) [![Installs](https://flat.badgen.net/vs-marketplace/i/flyfly6.terminal-in-status-bar?color=blue)](https://marketplace.visualstudio.com/items?itemName=flyfly6.terminal-in-status-bar) [![Rating](https://flat.badgen.net/vs-marketplace/rating/flyfly6.terminal-in-status-bar?color=blue)](https://marketplace.visualstudio.com/items?itemName=flyfly6.terminal-in-status-bar)                                                             |
| Better Comments         | [![Badge for version for Visual Studio Code extension](https://flat.badgen.net/vs-marketplace/v/aaron-bond.better-comments?icon=visualstudio&color=blue)](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments) [![Installs](https://flat.badgen.net/vs-marketplace/i/aaron-bond.better-comments?color=blue)](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments) [![Rating](https://flat.badgen.net/vs-marketplace/rating/aaron-bond.better-comments?color=blue)](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)                                                                                     |

[vsc essentials]: https://marketplace.visualstudio.com/items?itemName=Gydunhn.vsc-essentials
[here]: https://marketplace.visualstudio.com/items?itemName=Gydunhn.vsc-essentials
[This extension]: https://open-vsx.org/extension/Gydunhn/vsc-essentials-core
[open-vsx.org]: https://open-vsx.org/