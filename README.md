# Industrial Organization Models (Excel + VBA)

Excel toolkit with ~20 industrial organization models: mergers, price discrimination, vertical differentiation, platforms, collusion, entry barriers and auctions. Equilibria are solved with Solver and automated with VBA macros, with Monte Carlo risk simulation and sensitivity analysis on the assumptions.

![Home sheet](assets/home-sheet.png)

Each model lives in its own sheet: change the assumptions (demand, costs, taxes, number of firms, etc.), run the macro button, and read prices, quantities, profits and welfare effects next to the charts. The home sheet (`Inicio`) links to every module.

> **Language note:** the workbook interface (sheet names and labels) is in Spanish.

## Modules

| Block | Sheets | What it covers |
|---|---|---|
| **Taxes and market structure** | `Lineales`, `No lineales` | Specific and ad-valorem taxes under perfect competition, symmetric oligopoly and monopoly, with linear and non-linear demand |
| **Sensitivity** | `Sensibilidad` | Effect of elasticity, taxes, number of firms, market size and cost structure (constant, linear, quadratic) on price, quantity, profit and markup |
| **Mergers (M&A)** | `Cournot`, `Bertand`, `Efectos` | Pre/post-merger simulation under Cournot and differentiated Bertrand; changes in price, quantity, profit, consumer surplus, welfare and HHI; merger screens (CMCR, GUPPI, UPP, IPR) with efficiency synergies |
| **Price discrimination** | `Discriminacion` | Uniform pricing vs. third-degree (segmentation), second-degree (bundles) and two-part tariffs |
| **Stochastic risk** | `Riesgo` | Monte Carlo simulation (5,000 draws, Solver re-optimized in each one) of profits and prices: min, mean, max, deviation and probability of loss |
| **Multiproduct firms** | `Multiproducto` | Cannibalization, markups, Lerner indices and gains from coordination |
| **Product differentiation** | `Horizontal`, `Vertical` | Brand positioning with distance/crowding effects and market shares; quality-price competition (symmetric and asymmetric oligopoly) |
| **Two-sided platforms** | `Plataformas` | Monopoly and duopoly platforms with cross-network effects |
| **Innovation** | `Innovacion` | R&D investment under Cournot, Stackelberg and a research joint venture (RJV) |
| **Vertical relations** | `Integracion`, `Franquicia`, `Exclusividad` | Double marginalization and vertical integration, franchising, exclusive contracts with rescission clauses |
| **Property rights** | `Limites` | Grossman-Hart-Moore model: integrate vs. trade, upstream and downstream integration |
| **Collusion** | `Colusion` | Minimum discount factor for collusion (Cournot and differentiated Bertrand), with reporting lags |
| **Entry barriers** | `Barreras` | Capacity investment (accommodation vs. deterrence) and limit pricing |
| **Auctions** | `Subastas` | First- and second-price auctions, optimal reserve price, expected revenue |

## How to use

1. Download `industrial-organization-models.xlsm`.
2. Open it in desktop **Microsoft Excel** and **enable macros**.
3. Activate the **Solver** add-in (*File > Options > Add-ins > Manage Excel Add-ins > Solver Add-in*).
4. Go to the home sheet and click on a module.
5. Edit the inputs and press the module's button to recompute the equilibrium.

Some modules (such as `Riesgo`) run thousands of Solver optimizations and can take a few minutes.

## Requirements

- Microsoft Excel for Windows, with macros enabled
- Solver add-in
- The hidden sheet `Auxiliar` is used by the macros; do not delete it

## Author

**Marco Diaz de Sosa** · Economics student (UNLP)
[LinkedIn](https://www.linkedin.com/in/marco-diaz-de-sosa) · marcodiazdesosa@gmail.com

## License

MIT
