# TruEdge™ Color Themes — Overlay & HUD Palettes

This document outlines the branded color themes used across TruEdge overlays, diagnostics, and cockpit shells.

## 🎨 Theme Modules

| Theme File         | Purpose                            |
|--------------------|------------------------------------|
| `DarkMode.ts`      | HUD-safe tones for dark charts     |
| `ContextAware.ts`  | Regime-sensitive color logic       |
| `GlowZones.ts`     | Volatility tier glow overlays      |
| `TierPulse.ts`     | Pulse-state color transitions      |

## 🧠 Color Roles

| Role             | Description                          |
|------------------|--------------------------------------|
| `TrendUpColor`   | Used for bullish overlays            |
| `TrendDownColor` | Used for bearish overlays            |
| `VolatilityGlow` | Tier-based glow zones                |
| `HUDNeutral`     | Default HUD text and panel tone      |
| `RegimeActive`   | Highlight for active regime state    |

## 🧩 Theme Sync Logic

- All overlays reference `ThemeBridge.ts` for shared colors
- Shells use `ThemeBridge.ts` to sync HUD and panel tones
- Drops can override theme via `DropTheme.ts` if needed

## 🧪 Display Modes

| Mode     | Description                          |
|----------|--------------------------------------|
| `Classic`| Default branded palette              |
| `Silent` | Minimal overlays, HUD only           |
| `Glow`   | Full tier glow zones active          |

## 📝 License

MIT — remix, recolor, and build your legacy.
