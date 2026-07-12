# Workspace Notes

## What to Upload

For a public release, upload the release artifacts and documentation only:

- `overleaf-theme-pro-ultra-1.0.0.vsix`
- `overleaf-theme-pro-ultra-1.0.0-source.zip`
- `README.md`
- `01_COLOR_TABLE.md`
- `02_KNOWN_LIMITATIONS.md`
- `03_CHANGELOG.md`
- `04_THIRD_PARTY_NOTICES.md`
- `05_LICENSE.md`
- `06_WORKSPACE.md`

Do not upload temporary analysis folders, local editor backups, unpacked audit folders, screenshots, or machine-specific configuration files.

## Source Package Layout

The source zip expands to an `extension` folder. That folder is the clean editable source for the VS Code extension:

- `package.json`: extension manifest.
- `extension.js`: VS Code command implementation.
- `themes/`: color theme JSON.
- `syntaxes/`: TextMate injection grammar.
- `*.md`: public documentation.

## Installed Extension vs Source

Installing the VSIX copies the extension into VS Code's extension storage. Editing an installed copy does not update the source package automatically.

For future development, edit the clean source folder, rebuild the VSIX, then reinstall the new package.
