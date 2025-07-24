# TruEdge™ Contributor Guide

Welcome to the cockpit. This guide outlines how to contribute modules, drops, overlays, and orchestration shells to the TruEdge ecosystem.

## 🧩 Contribution Types

- **Modules**: Overlays, diagnostics, orchestration shells
- **Drops**: `.tru` presets for scoring, overlays, or scan logic
- **Docs**: README scaffolds, orchestration commentary, version logs
- **Themes**: Color palettes and HUD display logic

## 🛠️ Standards & Naming

| Type      | Format                          | Notes                          |
|-----------|----------------------------------|--------------------------------|
| Module    | `TruEdge_ModuleName_vX.Y.ts`     | Versioned, orchestration-safe |
| Drop      | `DropType_ModuleName.ts`         | Stored in `DropVault/drops/`  |
| Theme     | `ThemeName.ts`                   | Stored in `DropVault/themes/` |
| Docs      | `README_Scaffold_*.md`           | Stored in `ReadmeKit/`        |

## 🔧 Coding Guidelines

- Use toggle inputs for all overlays and diagnostics
- Default all toggles to `no` or `false` for safe shell loading
- Include header block with author, version, and description
- Use `#region` comments to visually separate logic blocks

## 🔗 Orchestration Integration

- All modules should sync regime via `RegimeBridge.ts`
- Drops must be compatible with `DropManager.ts`
- Shells must support scan/export routing via `LauncherShell.ts`

## 📎 How to Submit

1. Fork the relevant repo (e.g. `TruEdge_Overlays`)
2. Add your module or drop using proper naming
3. Include a matching README or `ABOUT_THIS_DROP.md`
4. Submit a pull request with a clear description

## 📝 License

MIT — remix, extend, and build your legacy.
