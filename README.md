# vsassist.new

This is copy of BoHomola/vsassist.nvim that has now been Archived with little changes.
Neovim colour scheme strongly inspired by The Cherno's Visual Studio colour scheme. It's a mix of VSCode, VSAssist (Visual Assist - VS extension) and Gruvbox.

Code based on [vsassist.nvim](https://github.com/BoHomola/vsassist.nvim) theme, which is based on [vscode.nvim](https://github.com/Mofiqul/vscode.nvim).

Scheme works with lsp semantic tokens.

## Preview

![preview](showcase/cpp/Showcase.png?)


## Usage

Install via package manager

```lua
-- Packer:
use("komilazio/vsassist.new")
```

Config (same as in vscode.nvim):

```lua
require("vsassist").setup({
    -- Enable transparent background
    transparent = true,

    -- Enable italic comment
    italic_comments = true,

    -- Disable nvim-tree background color
    disable_nvimtree_bg = true,

    -- Override colors (see ./lua/vsassist/colors.lua)
    color_overrides = {
        vscLineNumber = '#FFFFFF',
    },
})
```

```lua

vim.cmd("colorscheme vsassist")
```
