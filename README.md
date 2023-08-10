# My neovim only necessary things config

This is my third attempt at configuring neovim. As the name suggests this version of the configuration only includes things that I would term as absolute essentials for having a neovim setup for the purpose of programming and coding.  
This is configuration is not meant to be used for non-programmers (though they can as there are plugins that even they would benefit from).  
The reason to keep things at a bare minimum is to keep the neovim startup time as low as possible and easy maintaibality of the config.  
That is also the reason why I choose to keep everything in a single file.

## Plugin and list of plugins used
- Plugin manager: Lazy.nvim [lazy.nvim github repository](https://github.com/folke/lazy.nvim)  
This is the plugin that people have been moving to from packer.nvim since it is now archived. It also has the features of lazy loading plugins withuot any configuration required by the user apart from the default.  You can also check out the [lazyvim](https://www.lazyvim.org/) if you want something that is already all setup with documentation.
- telescope.nvim (plenary.nvim as dependency)
- treesitter playground
- nvim-treesitter
- undotree
- lsp-zero.nvim
    - nvim-lspconfig
    - mason.nvim
    - manson-lspconfig.nvim
    - nvim-cmp
    - cmp-nvim-lsp
    - LuaSnip
- neovim-ayu

### File searching and fuzzy finding
[telescope.nvim](https://github.com/nvim-telescope/telescope.nvim)
For this telescope.nvim is used. It is easy to use and only has one dependency `ripgrep` which can be installed by package-manager of your operating system (yes, even on windows or macos). The default keybindings make sense based on mnemonics.

### LSP and code completion
The most simple way to setup LSP and code completion was introduced to me by ThePrimeagen and this article written by VonHeikemen who wrote the lsp-zero plugin [article](https://dev.to/vonheikemen/getting-started-with-neovims-native-lsp-client-in-the-year-of-2022-the-easy-way-bp3)

### Colourscheme
You can use any colorscheme you want. I added a colourscheme to differentiate between when I am using the shell and when I am using neovim visually without having to read anything on the screen.

### Why everything in a single file?
- To make it easy to understand.
- I can't understand and get seperate files to work with lazy.nvim.
- **Yeah the second reason is not compelling I know.**
