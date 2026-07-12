# Overleaf Theme Pro Ultra 1.0.0

Overleaf Theme Pro Ultra is a VS Code theme package for people who prefer writing LaTeX locally but want an editor experience closer to Overleaf.

It customizes three parts of VS Code:

- LaTeX syntax highlighting: prose stays black, text commands are blue, math content is green, math commands are purple, and math braces/brackets follow Overleaf-like rules.
- Workbench appearance: tabs, breadcrumbs, sidebar text, editor selection, line highlight, and split borders are tuned toward an Overleaf-style writing workspace.
- Typography commands: the extension adds commands to apply and restore an Overleaf-inspired editor font, size, line height, cursor, tab size, and word wrap setup.

This release includes the installable VSIX, clean source package, color table, known limitations, changelog, third-party notices, license notes, and workspace notes.

## Files

- `overleaf-theme-pro-ultra-1.0.0.vsix`  
  Installable VS Code extension package.

- `overleaf-theme-pro-ultra-1.0.0-source.zip`  
  Clean source package for development and redistribution review.

- `01_COLOR_TABLE.md`  
  Color table for LaTeX token colors and UI colors.

- `02_KNOWN_LIMITATIONS.md`  
  VS Code theme API limits and behavior that cannot be fully matched with Overleaf.

- `03_CHANGELOG.md`  
  Release history.

- `04_THIRD_PARTY_NOTICES.md`  
  Source and attribution notes for the original theme, Overleaf, and VS Code grammar behavior.

- `05_LICENSE.md`  
  License and redistribution notes.

- `06_WORKSPACE.md`  
  Notes on what belongs in a public release and how to continue development from the source package.

## Install the VSIX

Install from VS Code:

1. Open the Extensions view.
2. Click the `...` menu.
3. Choose `Install from VSIX...`.
4. Select `overleaf-theme-pro-ultra-1.0.0.vsix`.
5. Reload VS Code if prompted.

Install from a terminal:

```bash
code --install-extension overleaf-theme-pro-ultra-1.0.0.vsix
```

## Enable the Theme

1. Run `Preferences: Color Theme`.
2. Select `Overleaf Theme Pro Ultra`.
3. Run `Overleaf Theme Pro Ultra: 应用 Overleaf 推荐排版` from the command palette.

To undo the typography changes, run `Overleaf Theme Pro Ultra: 恢复修改前排版`.

## Privacy Check

The public `.vsix` and source package were rebuilt from a clean staging directory. They should not contain local user paths, local project paths, Overleaf project IDs, editor backup files, screenshots, or machine-specific VS Code settings.
