# Industrial Organization Models (Excel + VBA)

Excel toolkit with ~20 industrial organization models: mergers, price discrimination, vertical differentiation, platforms, collusion, entry barriers and auctions. Equilibria are solved with Solver and automated with VBA macros, with Monte Carlo risk simulation and sensitivity analysis on the assumptions.

![Home sheet](IO-models-preview.png)

## Navigation

The workbook is built to be explored by clicking, no need to hunt through sheet tabs:

- **Home sheet (`Inicio`):** every blue button is a hyperlink that takes you straight to its module.
- **Sub-menus:** `Fusiones`, `Diferenciacion` and `Rel. Vert.` are hubs with their own buttons for the models inside them.
- **Back buttons:** every sheet has an `INICIO` / `ATRAS` button to return to the previous menu.
- **Recalculate buttons:** each model has a `Recalcular equilibrios` button (VBA macro) that re-solves it after you change the assumptions.

> **Language note:** the workbook interface (sheet names and labels) is in Spanish.

## Modules

| Home button | Sheet(s) | What it covers |
|---|---|---|
| **Impuestos** (linear) | `Lineales` | Specific and ad-valorem taxes under perfect competition, symmetric oligopoly and monopoly, with linear demand |
| **Impuestos** (non-linear) | `No lineales` | Same market structures with constant-elasticity demand and quadratic costs |
| **Sensibilidad** | `Sensibilidad` | Effect of elasticity, taxes, number of firms, market size and cost structure (constant, linear, quadratic) on price, quantity, profit and markup |
| **Fusiones (M&A)** | `Cournot`, `Bertand`, `Efectos` | Pre/post-merger simulation with homogeneous (Cournot) and differentiated (Bertrand) products; changes in price, quantity, profit, consumer surplus, welfare and HHI; price-effect screens (CMCR, GUPPI, UPP, IPR) with efficiency synergies |
| **Discriminación de precios** | `Discriminacion` | Uniform pricing vs. third-degree (segmentation), second-degree (bundles) and two-part tariffs |
| **Riesgo estocástico** | `Riesgo` | Monte Carlo simulation (5,000 draws, Solver re-optimized in each one) of profits and prices: min, mean, max, deviation and probability of loss |
| **Multiproducto** | `Multiproducto` | Cannibalization, markups, Lerner indices and gains from coordination |
| **Diferenciación** | `Horizontal`, `Vertical` | Brand positioning with distance/crowding effects and market shares; quality-price competition (symmetric and asymmetric oligopoly) |
| **Plataformas** | `Plataformas` | Two-sided markets: monopoly and duopoly platforms with cross-network effects |
| **Innovación** | `Innovacion` | R&D investment under Cournot, Stackelberg and a research joint venture (RJV), with a comparison table |
| **Relaciones verticales** | `Integracion`, `Franquicia`, `Exclusividad` | Double marginalization and vertical integration, franchising (two-part tariff), exclusive contracts with rescission clauses |
| **Subastas** | `Subastas` | First- and second-price auctions, optimal reserve price, expected revenue |
| **Colusión** | `Colusion` | Minimum discount factor for collusion (Cournot and differentiated Bertrand), with reporting lags |
| **Barreras a la entrada** | `Barreras` | Capacity investment (accommodation vs. deterrence) and limit pricing |
| **Property rights** | `Limites` | Grossman-Hart-Moore model: integrate vs. trade, upstream and downstream integration |

## How to use

1. Download `industrial-organization-models.xlsm`.
2. Open it in desktop **Microsoft Excel** and **enable macros**.
3. Activate the **Solver** add-in (*File > Options > Add-ins > Manage Excel Add-ins > Solver Add-in*).
4. On the home sheet, click the module you want.
5. Edit the inputs and press `Recalcular equilibrios` to recompute.

Some modules (such as `Riesgo`) run thousands of Solver optimizations and can take a few minutes.

## Requirements

- Microsoft Excel for Windows, with macros enabled
- Solver add-in
- The hidden sheet `Auxiliar` is used by the macros; do not delete it
