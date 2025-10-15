# transparent.nvim

If you love transparent term, but your favourite Neovim color scheme doesn't

If your are vim (Not neovim) user, Use [vim-transparent][] instead.

[vim-transparent]: https://github.com/tribela/vim-transparent


# Screenshots

With transparent.nvim (example color scheme is **tokyonight**)

<img width="1367" height="768" alt="screenshot_1760491605" src="https://github.com/user-attachments/assets/9c9c5932-3f52-41bc-8e80-c990dfeb50c5" />



Without vim-transparent

<img width="1366" height="768" alt="screenshot_1760493192" src="https://github.com/user-attachments/assets/77de8d62-847a-4f83-8aab-1ab5efd7522e" />


# Fix : (LazyUI)

<p>The Lazy UI and other parts were not working with original <code>transparent.nvim</code> configs, which are now working.</p>

<p align=center>
<img width="1367" height="769" alt="screenshot_1760491673" src="https://github.com/user-attachments/assets/5cf56adb-db77-4ed5-9a63-97c0a55ba758" />

<img width="1366" height="768" alt="screenshot_1760491841" src="https://github.com/user-attachments/assets/83c1a0a2-57a0-47ab-a596-c525de8f3738" />

</p>


[tokyonight]: https://github.com/folke/tokyonight.nvim


## Installation

### [lazy.nvim](https://github.com/folke/lazy.nvim)

<p>Make a file in <code>~/.config/nvim/your-plugins-folder/transparent.lua</code> and paste the snippet and launch <code>nvim</code>.<br>If the plugin does not load try running <code>:Lazy sync</code>.</p>

```lua
return {
    'tanshen-kun/transparent.nvim',
    lazy = false,
    config = true,
}
```

## Configuration

```lua
{
    auto = true, -- Automatically applies transparent
    extra_groups = {}, -- If you want to add some groups to be transparent. eg: { 'Pmenu', 'CocFloating' }
    excludes = {}, -- If you want to excludes from default transparent groups. eg: { 'LineNr' }
}
```

## Usage

transparent.nvim automatically transparent all of highlight settings.

You can disable it by `:TransparentDisable` and re-enable it by `:TransparentEnable`, Toggle it by `:TransparentToggle`
