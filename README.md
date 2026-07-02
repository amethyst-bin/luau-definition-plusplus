# LuauDefinition++

## How to connect
### VScode / Codium
- Install LSP [Link](https://marketplace.visualstudio.com/items?itemName=JohnnyMorganz.luau-lsp)
- Create `.vscode`
- Clone repo into `.vscode` folder
- Create `settings.json` in `.vscode`
```jsonc
// .vscode/settings.json
{
  "luau-lsp.types.definitionFiles": [
    ".vscode/luau-definition-plusplus/aio.d.luau", // executors types
    ".vscode/luau-definition-plusplus/globalTypes.d.luau", // all roblox types
  ],

}
```
- `Ctrl + Shift + P` > Luau: Reload Language Server
### Zed
- idk
- if it worked for zen pls dm me in discord i wanna know `tinytosha`

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
