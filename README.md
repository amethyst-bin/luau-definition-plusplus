# LuauDefinition++

## How to connect
- Create `.vscode`
- Put `aio.d.luau` in `.vscode`
- Create `settings.json` in `.vscode`
```jsonc
// .vscode/settings.json
{
  "luau-lsp.types.definitionFiles": [
    ".vscode/aio.d.luau",
  ],

}
```
- `Ctrl + Shift + P` > Luau: Reload Language Server

## Feutares
- All injectors env libs (unc, sunc and more)
- [NullUI](https://github.com/ginzuss/nullui) Support

## How use NullUI
```luau
-- Instead of
local NullLib = loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/ginzuss/nullui/refs/heads/main/NullUI.lua"))()
-- Use
local NullLib = loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/ginzuss/nullui/refs/heads/main/NullUI.lua"))() :: NullUILibrary
```
