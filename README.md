# Model-Based Visual–Tactile Control for Precision Dexterous In-Hand Tweezer Manipulation

A single-page reading edition of the paper, typeset in a **Kandinsky / Bauhaus constructivist** style.

## What this is

Where [Part 1](https://fangde.github.io/kandinsky-tweezers/) used pure analytical kinematics, this
paper splits control into three roles that stay out of each other's way:

| Role | Answers | Mechanism |
|---|---|---|
| **Model** | how should the fingers move? | analytical hand–tool kinematics + a constrained QP |
| **Vision** | did the tool tip actually arrive? | measures the tweezer tip in Cartesian space, eats the model error |
| **Touch** | is the tool still securely grasped? | regulates internal grasp force in the null space |

The result is interpretable and needs no end-to-end learning. The paper's
5 → 4.6 → 4.93 → 4.99 → 5.00 mm convergence sequence is exactly the point: the model does not
have to be right the first time.

## Pages

| File | Edition |
|---|---|
| `index.html` | English (primary) |
| `zh.html` | 中文精读版 |

Both editions carry a switch chip in the hero meta row.

## Design

| Dimension | Approach |
|---|---|
| Palette | rice-paper `#F2EEE3` + charcoal `#131313` + Bauhaus primaries (vermilion `#DF3524` / chrome yellow `#F0C200` / ultramarine `#1D3FA6`), flat fills only |
| Type | Jost (geometric sans, Futura-adjacent) for display, Noto Sans SC for body, IBM Plex Mono for numerals |
| Layout | square corners, no gradients, no shadows, hard-edged rules; left spine, right section nav, tri-colour reading progress |
| Artwork | hero and inline plates are pure geometric compositions (circle / triangle / square / concentric arcs / hard diagonals) |
| Maths | every equation rendered live with KaTeX — selectable, copy-ready LaTeX |
| Motion | staggered hero reveal, scroll reveal, section tracking nav, `prefers-reduced-motion` aware |

## Files

```
.
├── index.html            # English edition (self-contained design system; CDN fonts + KaTeX only)
├── zh.html               # Chinese edition
├── assets/images/        # 5 Bauhaus plates
├── .nojekyll             # disable Jekyll
└── README.md
```

## Series

- [Part 1 — Analytical Modelling with a Locked Wrist](https://fangde.github.io/kandinsky-tweezers/)
- Part 2 (this page) — Visual positioning + tactile grasp

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Licence

The paper text and figures remain the property of the original authors; this repository only
presents the typography and reading experience.
