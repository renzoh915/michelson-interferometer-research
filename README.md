# Improving Fringe Readability in a 532 nm Michelson Interferometer

**Renzo Herrera**  
Undergraduate optics research, Montclair State University  
Research mentor: **Dr. Rodica Martin**

An engineering case study documenting the troubleshooting of a laboratory Michelson interferometer used to investigate temperature-dependent optical-path changes in TGG, CeF₃, and fused silica.

**[Read the three-page report (PDF)](Renzo_Herrera_Michelson_Interferometer_Case_Study.pdf)**

![June 4 and July 8 TGG interference traces](figures/tgg_before_after_clean.png)

## What I worked on

- Built, aligned, and repeatedly reconfigured a 532 nm Michelson interferometer.
- Installed shielding to reduce air movement around the optical paths, and improved sample positioning, mounting, and alignment.
- Soldered temperature-probe extensions and configured automatic multichannel temperature logging.
- Investigated plotting artifacts in IGOR Pro while assessing which fringe extrema could be counted.
- Compared exported early and later interference traces to document improved fringe readability.

## What this case study demonstrates

Later traces contain more visually distinguishable interference fringes than selected early trials. The work demonstrates iterative optical-instrument troubleshooting, **not** a controlled quantitative measurement of noise reduction, uncertainty, or absolute accuracy. The environmental disturbances addressed here are distinct from the sensing and control noise mechanisms in LIGO detectors.

The report also documents preliminary fringe-derived values from the original laboratory notes. Their underlying coefficient convention, some summary calculations, and at least one recorded temperature interval require reconciliation before these numbers are used as validated intrinsic material properties. The original exported plots, rather than reconstructed numerical measurements, are included.

## Repository contents

- `Renzo_Herrera_Michelson_Interferometer_Case_Study.pdf` — report intended for reading or sharing.
- `main.tex` — fully editable LaTeX source.
- `figures/` — schematic, original-poster photo crops, and panels assembled from original exported plots.
- `source_plots/` — original IGOR Pro plot exports used in the included comparisons.

## Build the PDF

Use a standard LaTeX installation with `extarticle`, `graphicx`, `amsmath`, `booktabs`, `microtype`, `xcolor`, `tabularx`, `float`, `fancyhdr`, `titlesec`, `enumitem`, and `hyperref`. The report does **not** require a custom journal class.

```bash
latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex
```

Alternatively, run `pdflatex main.tex` twice. On Overleaf, upload `main.tex` and `figures/`, then compile with pdfLaTeX.

## Research attribution and figure provenance

Research carried out at Montclair State University under Dr. Rodica Martin's mentorship. The source plot exports came from the original undergraduate research records. The instrumentation photographs are low-resolution crops from the associated research poster; the schematic is a conceptual illustration, not a record of exact optical geometry. The comparison panels only arrange original exports side-by-side and do not change the recorded curve values.

This independent portfolio report is **not** an official LIGO publication and does not claim LIGO detector calibration. Confirm that research photographs and shared materials are cleared for public redistribution before making a repository public.
