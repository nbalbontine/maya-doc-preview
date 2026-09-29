# Maya doc preview (GitHub Pages)

Public, shareable diagrams for the [Maya PDLC stakeholder brief](https://github.com/nbalbontine/maya-doc/blob/main/docs/maya-pdlc-stakeholder-brief.md).

## Live site

After GitHub Pages is enabled, open:

**https://nbalbontine.github.io/maya-doc-preview/pdlc-diagrams.html**

Section anchors (for decks and the brief):

| Section | URL |
| :--- | :--- |
| Scattered today | `.../pdlc-diagrams.html#scattered` |
| Old vs new | `.../pdlc-diagrams.html#contrast` |
| Repo chain | `.../pdlc-diagrams.html#chain` |
| Artifacts | `.../pdlc-diagrams.html#artifacts` |
| Update cascade | `.../pdlc-diagrams.html#cascade` |
| Roles flow | `.../pdlc-diagrams.html#roles` |

## Layout

| Path | Purpose |
| :--- | :--- |
| `pdlc-diagrams.html` | Main page (Mermaid diagrams) |
| `index.html` | Redirects to `pdlc-diagrams.html` |
| `css/site.css` | Styles — extend here for layout and branding |

Diagram source lives in `<pre class="mermaid">` blocks inside `pdlc-diagrams.html`. Mermaid loads from jsDelivr (internet required once per visit).

## Local preview

```bash
python3 -m http.server 8787
# open http://localhost:8787/pdlc-diagrams.html
```

## Sync from `maya-doc`

The canonical product dossier lives in [maya-doc](https://github.com/nbalbontine/maya-doc). When you update diagrams in `docs/visuals/pdlc-diagrams.html` there, copy or merge changes into this repo and push `main` — Pages redeploys automatically.
