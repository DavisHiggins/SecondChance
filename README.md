<p align="center">
  <a href="https://secondc.vercel.app"><img src="assets/hero.svg" width="100%" alt="SecondChance: earlier attention, shorter waits, more animals home. Animated cover with the SecondChance logo inside turning teal rings beside a scrolling support queue of animal cards." /></a>
</p>

<h1 align="center">SecondChance</h1>

<p align="center"><strong>A predictive-analytics platform that turns animal long-stay risk into earlier, more focused shelter support.</strong></p>

<p align="center">
  <a href="https://secondc.vercel.app"><img src="assets/btn-open.svg" height="44" alt="Open SecondChance" /></a>&nbsp;
  <a href="https://www.higginsd.com/work/secondchance"><img src="assets/btn-case.svg" height="44" alt="Case study" /></a>&nbsp;
  <a href="https://davishiggins.com"><img src="assets/btn-dh.svg" height="44" alt="Davis Higgins" /></a>
</p>

<p align="center"><sub>Live · UNC Charlotte team project · Website by Davis Higgins</sub></p>

---

## See it in motion

<p align="center">
  <img src="assets/demo.gif" width="880" alt="Screen recording of the SecondChance support queue: filtering to cats waiting 30 or more days, switching to card view, and expanding why outreach is suggested for one animal." />
</p>

<p align="center"><sub>Real capture of secondc.vercel.app/queue using the City of Austin's public shelter records. <a href="assets/demo.png">Static frame</a></sub></p>

## What it does

- **A support queue that leads with the wait.** Open stays are ranked by their likelihood of a long stay, with actual days waiting beside each one, and filters for species, life stage, and wait time.
- **Records with their context.** Each animal's page shows the stay timeline, what was known at intake, and a suggested kind of support.
- **A weekly outreach planner.** Staff set their capacity, choose actions, and export or print a plan for the week.

## Why it exists

Shelters make time-sensitive decisions with limited staff, foster homes, and hours in the day. The people doing the work know why some animals wait longer, but reviewing every case at the right moment is hard.

The project has one rule, and it appears on every operational page: **a high predicted long-stay risk is a request for more help, not less.** Scores route photography, profile improvements, foster recruitment, and outreach toward animals who need it.

## My contribution

SecondChance is a four-person UNC Charlotte predictive analytics project built with Bennett Shearin, Seth Sumter, and Hunter Pace. The research and modeling were shared team work. My part:

- Designing and building the web application: dashboard, support queue, record browser, outreach planner, impact page, and methodology pages
- Presenting the team's work clearly, with observed outcomes, predictions, and planning assumptions kept visibly separate
- The project's presentation

<details>
<summary><strong>How it's put together</strong></summary>

<br />

```mermaid
flowchart TB
    A[City of Austin<br/>public shelter records] --> V[Validated, paired stays]
    V --> M[Team-built prediction model]
    M --> Q[Queue · Records · Planner]
    V --> S[Defined metrics]
    S --> D[Dashboard]
```

| Decision | Why |
|---|---|
| **Predictions made at intake** | Estimates use only what was known when an animal arrived, so they reflect a real decision point. |
| **Every metric defined once** | Each figure has one definition used everywhere it appears, so the dashboard, records, and glossary always agree. |
| **Fresh data, clearly dated** | The site tracks when the source data was last updated and says so when the feed runs late. |

</details>

## Screens

<table>
  <tr>
    <td width="62%"><img src="assets/screenshot-dashboard.png" alt="SecondChance shelter overview: 'Earlier attention. Shorter waits. More animals home.' with the live open-stay count from Austin's feed." /></td>
    <td rowspan="2" width="38%" align="center"><img src="assets/screenshot-mobile.png" width="300" alt="SecondChance support queue on a phone, headed 'Animals that may need extra support'." /></td>
  </tr>
  <tr>
    <td><img src="assets/screenshot-model.png" alt="SecondChance 'Understand the data and predictions' page explaining the model's evaluation in plain language." /></td>
  </tr>
</table>

<sub>Shelter overview · The data and predictions, in plain language · Support queue on mobile</sub>

## Technology

| Layer | Technology |
|---|---|
| Web app | Next.js, React, TypeScript, Tailwind CSS |
| Modeling | Python |
| Motion | GSAP, Lenis |
| Hosting | Vercel |

---

<p align="center">
  <a href="https://secondc.vercel.app"><img src="assets/btn-open.svg" height="44" alt="Open SecondChance" /></a>&nbsp;
  <a href="https://github.com/DavisHiggins"><img src="assets/btn-more.svg" height="44" alt="More of my work" /></a>
</p>

<p align="center"><sub>© 2026 Davis Higgins. Shelter data: City of Austin Open Data Portal.</sub></p>
