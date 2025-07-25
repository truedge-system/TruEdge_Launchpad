# Orchestration Map Legend — TruEdge™ RealSuite

This legend explains the flow arrows, module types, and regime sync logic used in `Orchestration_Map.md`.

---

## 🔄 Flow Arrows

- `→` : Direct signal or overlay flow
- `↔` : Bidirectional sync (e.g. regime or metadata)
- `⇄` : Feedback loop (e.g. diagnostics or drop routing)

---

## 🧩 Module Types

| Type              | Description                                      |
|-------------------|--------------------------------------------------|
| Shell             | Orchestration interface (e.g. `FusionMaster.ts`) |
| Overlay           | Visual logic (e.g. `CockpitView.ts`)             |
| Compiler          | Drop logic + GitHub sync                         |
| Execution         | Trade logic + journaling                         |
| Diagnostic        | HUD commentary + signal feedback                 |
| Theme             | Visual assets + tone engine                      |

---

## 🧠 Regime Sync Logic

All modules reference `RegimeBridge.ts` for shared context:

- **Tier-aware overlays** adapt to regime state
- **Signal engines** toggle based on regime filters
- **Diagnostics** display only when regime conditions match

This ensures orchestration clarity across all shells and overlays.
# Orchestration Map Legend — TruEdge™ RealSuite

This legend explains the visual flow, module types, and regime sync logic used in `Orchestration_Map.md`.

---

## 🔄 Flow Arrows

| Symbol | Meaning                                 |
|--------|------------------------------------------|
| `→`    | Direct signal or overlay flow            |
| `↔`    | Bidirectional sync (e.g. regime, metadata)|
| `⇄`    | Feedback loop (e.g. diagnostics, drops)  |

---

## 🧩 Module Types

| Type        | Description                                      |
|-------------|--------------------------------------------------|
| Shell       | Orchestration interface (e.g. `FusionMaster.ts`) |
| Overlay     | Visual logic (e.g. `CockpitView.ts`)             |
| Compiler    | Drop logic + GitHub sync                         |
| Execution   | Trade logic + journaling                         |
| Diagnostic  | HUD commentary + signal feedback                 |
| Theme       | Visual assets + tone engine                      |

---

## 🧠 Regime Sync Logic

All modules reference `RegimeBridge.ts` for shared context:
👉 See [Orchestration_Map_Legend.md](docs/Orchestration_Map_Legend.md) for flow key and module types.
- **Tier-aware overlays** adapt to regime state
- **Signal engines** toggle based on regime filters
- **Diagnostics** display only when regime conditions match

This ensures orchestration clarity across all shells and overlays.
