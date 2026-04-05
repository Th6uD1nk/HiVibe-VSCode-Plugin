# HighVibe

HighVibe is a VS Code extension that provides **syntax highlighting** for the HighVibe DSL (`.hvibe` files).

## Features

- Different colors for `"..."` strings (developer-facing) and `` `...` `` strings (LLM-direct)  
- Catalog keys and subkeys in **green**  
- Schema keys in **blue**  
- Keywords like `MUST BE`, `MUST ALWAYS`, `MUST NEVER` in **red**  
- Numbers and punctuation highlighted for clarity

## Usage

1. Install the extension in VS Code.  
2. Open a `.hvibe` file.  
3. Enjoy proper syntax highlighting for HighVibe projects.

## Installation

### Install vsce if not already installed
```bash
npm install -g @vscode/vsce
````

### Package the extension

```bash
vsce package
```

### Install the generated VSIX locally

```bash
code --install-extension hvibe-0.0.1.vsix
```

### Select the HighVibe theme

After installation, open VS Code, press `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS), type **Color Theme**, and select **HighVibe Theme** to activate syntax highlighting.


## Minimal Example

```hvibe
{
  hvibe_version: "0.1.0",
  app: "my-app",
  description: `This is a simple demo`,
  stack: [`javascript`],
  catalog: {
    logic: {
      rocket_arc: `linear interpolation from bottom to top`
    }
  }
}
