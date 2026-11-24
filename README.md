# hodge-theory-notes

Two expository papers on the Hodge theory of smooth complex projective varieties, with their LaTeX sources and a shared bibliography. They began as notes written while reading Voisin's *Hodge Theory and Complex Algebraic Geometry* and the literature around it. Neither paper contains new results.

## Contents

| File | Title |
| --- | --- |
| `gaga_kahler_lefschetz.tex` | Notes on Analytification, GAGA, Kähler Identities, and Lefschetz Theory |
| [Notes on Analytification, GAGA, Kähler Identities, and Lefschetz Theory (PDF)](gaga_kahler_lefschetz.pdf) | Notes on Analytification, GAGA, Kähler Identities, and Lefschetz Theory |
| `hodge_classes_algebraic_cycles.tex` | Hodge Classes and Algebraic Cycles |
| `references.bib` | Bibliography used by both papers |

### Notes on Analytification, GAGA, Kähler Identities, and Lefschetz Theory

The notes start from the analytification functor and Serre's GAGA theorem and show that a smooth projective variety has a compact Kähler analytification. The Kähler identities are proved in holomorphic normal coordinates, and $\Delta_d = 2\Delta_{\bar\partial}$ together with the elliptic Hodge theorem gives the Hodge decomposition. The Lefschetz operators give the space of harmonic forms a finite-dimensional $\mathfrak{sl}_2$-representation, yielding Hard Lefschetz and the primitive decomposition. The last sections compute the Hodge diamond of a smooth quintic threefold and show that cup product with the hyperplane class,
$h\smile(-):H^2(X,\mathbb{Z})\to H^4(X,\mathbb{Z})$, has image of index five.

### Hodge Classes and Algebraic Cycles

This paper states the rational Hodge conjecture, constructs the cycle-class map, and explains why the class of a subvariety has type $(p,p)$. It proves the divisor and curve cases of the rational Hodge conjecture. Together with the codimension-zero and top-degree cases, these establish the conjecture for smooth complex projective varieties of dimension at most three. On a smooth quintic threefold, a plane-section curve represents five times the integral generator of $H^4(X,\mathbb Z)$. Dividing its class by five gives the rational representative used in the Lefschetz argument.

The later sections survey what is known beyond these cases: the failure of the integral and Kähler versions (Atiyah–Hirzebruch, Kollár, Voisin), the algebraicity of Hodge loci (Cattani–Deligne–Kaplan), absolute Hodge classes, the generalized Hodge conjecture, and Markman's recent work on abelian varieties as presented in Voisin's Bourbaki exposé. The general conjecture remains open.

### How the two papers fit together

The first paper supplies the analytic input for the second: the Hodge decomposition, Hard Lefschetz over $\mathbb{Q}$, and the cohomology of the quintic threefold. The second cites the first for these by section number, and the first refers to the second for the Lefschetz $(1,1)$ theorem and for curve classes on the quintic. Either paper can be read on its own.

## Building

Both papers compile with pdfLaTeX and BibTeX (`amsalpha` style). With `latexmk`:

```bash
latexmk -pdf gaga_kahler_lefschetz.tex
latexmk -pdf hodge_classes_algebraic_cycles.tex
```

The sources use standard classes and packages distributed with TeX Live.
They have been tested with TeX Live 2023.

## Main references

- C. Voisin, *Hodge Theory and Complex Algebraic Geometry I and II*,
  Cambridge University Press, 2002–2003.
- P. Griffiths and J. Harris, *Principles of Algebraic Geometry*, Wiley, 1978.
- J.-P. Serre, *Géométrie algébrique et géométrie analytique*, Ann. Inst.
  Fourier 6 (1956).
- W. Fulton, *Intersection Theory*, 2nd ed., Springer, 1998.
- P. Deligne, *The Hodge conjecture*, in *The Millennium Prize Problems*,
  Clay Mathematics Institute, 2006.

The full list is in `references.bib`.

## Corrections

Corrections and comments are welcome. Please open an issue.
