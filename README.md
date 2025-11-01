# fleeting-notes.nvim

A Neovim extension to quickly open up a markdown buffer and store your ideas. This extension is ideal for methods like [GTD](https://en.wikipedia.org/wiki/Getting_Things_Done).

## Installation

Remember to update the target file to use your own directory and target note.

lazy.nvim
```lua
{
    "alifoo/fleeting-notes.nvim",
    config = function()
        require("fleeting-notes").setup({ target_file = "~/your-folder/notes.md" })
        vim.keymap.set("n", "<leader>fn", ":Fn<CR>", { silent = true })
    end,
}
```

### Credits

This is my first nvim extension. All thanks to [@Code Sphere](https://www.youtube.com/@codingwithspherev) for providing excellent guiding.
