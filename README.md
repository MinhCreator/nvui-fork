# NvChad UI Plugin 

This ui plugin is fork from nvchad ui
- Docs at `:h nvui` 

## Install

- Create `lua/chadrc.lua` file that returns a table, can be empty table too.
- Table structure must be same as [nvconfig.lua](https://github.com/NvChad/ui/blob/v3.0/lua/nvconfig.lua)

In your plugins file
```lua
 "nvim-lua/plenary.nvim",
 { "nvim-tree/nvim-web-devicons", lazy = true },

 {
   "nvchad/ui",
    config = function()
      require "nvchad" 
    end
 },

 {
    "nvchad/base46",
    lazy = true,
    build = function()
      require("base46").load_all_highlights()
    end,
 },

 "nvchad/volt", -- optional, needed for theme switcher
 -- or just use Telescope themes
```


## List of Features with screenshots 


## NvCheatsheet

- Auto-generated mappings cheatsheet module, which has a similar layout to that of CSS's masonry layout.
- It has 2 themes ( grid & simple )
![img](https://nvchad.com/features/nvcheatsheet.webp)
## NvThemePicker
- Choose your prefer builtin theme or integration external theme
[![IMAGE](https://img.youtube.com/vi/xytzreFq_us/0.jpg)](https://www.youtube.com/watch?v=xytzreFq_us)
# Credits

- Huge thanks to [@siduck](https://github.com/NvChad) for creating [nvchad-ui](https://github.com/NvChad/ui).