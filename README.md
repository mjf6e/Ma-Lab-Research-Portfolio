# Ma Lab Research Portfolio

A GitHub Pages resource site for the **Ma Laboratory** (Division of Surgical Sciences,
Department of Surgery, University of Virginia School of Medicine), built for new
students, lab members, and the general public to get oriented in the lab's three
research lines:

- **MG53 / TRIM72** — membrane repair biology
- **CitH3 & NETosis** — citrullinated histone H3 and neutrophil extracellular traps
- **MG29** — calcium signaling at the muscle triad junction

## Structure

```
_config.yml          Jekyll config (GitHub Pages builds this automatically)
_layouts/default.html Shared page shell: nav + footer
assets/style.css      Site styles
index.html            Home page
research/mg53.html
research/netosis-cith3.html
research/mg29.html
publications.html     Bibliography grouped by research line (PubMed-sourced)
funding.html           Current / recent NIH-funded projects
```

## Updating content

- **New publication:** add a `<li class="pub">` entry to the relevant section in
  `publications.html`, following the existing markup pattern (year, title, citation,
  PubMed + DOI links).
- **New funding item:** add a `<div class="fund">` block to `funding.html`.
- **Site-wide nav/footer:** edit `_layouts/default.html` once; it applies everywhere.

## Publishing

This repo is set up for GitHub Pages with Jekyll (the default GitHub Pages build,
no custom build step required). Enable it under **Settings → Pages → Build and
deployment → Source: Deploy from a branch**, and pick the branch this content lives
on (root directory).

## Sourcing notes

Publication and funding data were compiled from PubMed (`Jianjie Ma[Author]`
combined with each protein/pathway name) and from public institutional
announcements, linked at the point of use. This site summarizes and links to
primary sources; it does not reproduce full text from any external source.

<!-- build trigger: forcing a fresh Pages deployment after a stuck queued run -->
