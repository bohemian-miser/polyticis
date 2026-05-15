# Polyticis: Australian Federal Elections (2004–2026) in 4D Simplex Space

**[🚀 Explore the Live Interactive 3D WebGL Demo on GitHub Pages](https://bohemian-miser.github.io/polyticis/)**

![GitHub Pages Status](https://img.shields.io/badge/Deployment-Live_on_GitHub_Pages-54CCE3?style=for-the-badge&logo=github)
![AEC Data](https://img.shields.io/badge/Data_Source-AEC_Tally_Room_Archive-F49D22?style=for-the-badge)

---

## What is This Project?
**Polyticis** is an advanced psephological visualization that maps every Australian federal electorate across 8 election cycles (2004–2025) and early 2026 polling models into a **4-dimensional compositional simplex (3D regular tetrahedron)**.

By moving beyond traditional 2-party preferred (2PP) maps or static ternary plots, this model plots electorates in 3D barycentric space where the four corners represent 100% primary vote apexes for:
*   🔴 **Labor (ALP)**: Bottom-left ground vertex $(0,0,0)$.
*   🔵 **Coalition (LNP)**: Bottom-right ground vertex $(1,0,0)$.
*   🟠 **One Nation (ONP)**: Top vertical 3D elevation peak $(0.5, 0.289, 0.816)$.
*   ⚪ **Other / Greens / Teals**: Top-back ground corner $(0.5, 0.866, 0)$.

## Features
*   **89 Quarterly Time Steps (2004.00 to 2026.00)**: Scrub the interactive slider or click **Play** to watch all 150+ electorates smoothly migrate across 22 years of political history via WebGL time-lapse interpolation.
*   **Demographic Vulnerability & Defection Matrix (2026 Model)**: Grounded in early 2026 polling (YouGov/DemosAU) showing One Nation at 25%–32% nationally. Rather than a uniform additive swing, the 2026 model dynamically evaluates each seat's demographic vulnerability index ($\beta_d$) based on its 2025 actual performance. In highly vulnerable regional/working-class seats, disaffected conservative voters defect from LNP to ONP in massive numbers (defection rates up to 45%), while progressive metropolitan seats remain insulated on the ground floor.
*   **Psephological Lore Hardpoints**: Accurately models hard data events including David Farley's historic May 2026 Farrer by-election victory (**39.54% ONP**) and Barnaby Joyce's defection to One Nation in New England (**55% ONP**).

---

## Data Sources
1.  **AEC Tally Room Archive** ([results.aec.gov.au](https://results.aec.gov.au)): Official division-by-division candidate primary vote counts for the 2004, 2007, 2010, 2013, 2016, 2019, 2022, and 2025 federal elections.
2.  **Psephos Archive** ([psephos.adam-carr.net](http://psephos.adam-carr.net/)): Cross-referencing historical division boundaries and electoral lore.

## Running Locally
You can simply double-click `index.html` or `animated_tetrahedron.html` in any modern browser to explore the visualization locally (requires internet access to load the Plotly.js CDN library).

```bash
# Clone repository
git clone https://github.com/bohemian-miser/polyticis.git
cd polyticis

# Open in browser
open index.html
```

---
*Authored by bohemian-miser for the Polyticis Electoral Research Suite.*
