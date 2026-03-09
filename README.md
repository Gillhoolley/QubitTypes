# Global Qubit Innovation Atlas

This project contains a standalone interactive webpage that visualizes global qubit technology development on a rotating globe.

Live report: https://impactquantum.com/QubitTypes/

## What is implemented

- Rotating 3D globe with country-level highlighting
- Top navigation dropdown filter by qubit technology
- Color mapping for all 9 requested qubit types
- Hover interactions with:
  - Country name
  - Active qubit technologies
  - Companies/institutions
  - Government initiatives
- Side panel with summary stats and technology legend
- Mobile-responsive layout

## Main file

- `index.html`

Open `index.html` in a browser to run the visualization.

## Raw data folder convention

Use lowercase kebab-case for all `RawData` directories.

Current directories:

- `RawData/photonics`
- `RawData/semiconducting-qubits`
- `RawData/semiconductor-spin`
- `RawData/topological`
- `RawData/trapped-ion`

### Semiconductor folder merge note

`semiconducting-qubits` and `semiconductor-spin` currently overlap in scope.

- `semiconductor-spin` is a specific qubit modality (spin-based semiconductor qubits) and matches the taxonomy used by the visualization.
- `semiconducting-qubits` reads as a broader umbrella label and can duplicate records, country counts, and organization attribution if both are treated as separate peer categories.

Recommended approach:

- Keep `RawData/semiconductor-spin` as the canonical category for the current map/report taxonomy.
- Merge overlapping files from `RawData/semiconducting-qubits` into `RawData/semiconductor-spin`, or use `semiconducting-qubits` only as a temporary intake/staging folder before normalization.

## Qubit color mapping

- Photonic — Dark Green
- Topological — Dark Blue
- Ion Trap — Yellow
- Semiconductor Spin — Purple
- Superconducting — Orange
- Neutral Atom — Light Blue
- Quantum Dot — Red
- Diamond NV Center — Pink
- NMR — Neon Green

## Where to edit data and behavior

In `index.html`:

- Qubit labels/colors: around `const qubitConfig`
- Country/company/institution/initiative data: around `const qubitData`
- Country details rendering: around `function updateCountryPanel(...)`
- Globe setup and world map loading: around `async function init()`

## Data model used

Each qubit technology key in `qubitData` contains rows like:

```js
{
  iso3: "USA",
  country: "United States",
  orgs: ["Company A", "Institute B"],
  initiatives: ["Program X"]
}
```

A unified country profile is built from all technologies, so one country can appear in multiple qubit categories.

## Notes

- The current dataset is structured and ready to be replaced with your report-derived data.
- Globe/world geometry and rendering assets are loaded from public CDNs at runtime.
- Visual verification should be done by opening `index.html` locally.
