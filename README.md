# From Fluorescence to Imaging: How Optical Technologies Reveal Protein Information

从荧光到成像：光学技术如何“看见”蛋白质

## Overview

An undergraduate literature review and course presentation for **Introduction to Biomacromolecular Science** at Jiangnan University, presented on October 20, 2026.

From an optoelectronic engineering perspective, the presentation connects protein location, conformation and molecular interactions to measurable fluorescence signals. Its organizing question is how labeling, optical instrumentation and data interpretation work together to answer a biological question.

This is a literature-based educational project. The experimental results discussed below belong to the cited researchers; no new protein experiments, instrument validation or original image reconstruction were performed for this project.

## Topics Covered

| Topic | Focus in the presentation |
| --- | --- |
| Fluorescence labeling | GFP fusion, site-specific organic dyes and fluorescent antibodies connect a protein target to a detectable signal. Label size and attachment geometry affect interpretation. |
| Fluorescence lifetime imaging microscopy (FLIM) | Maps fluorescence decay characteristics across an image. Pulsed excitation with time-correlated single-photon counting (TCSPC) is one time-domain implementation; FLIM is not synonymous with TCSPC. |
| Förster resonance energy transfer (FRET) | Nonradiative donor-to-acceptor energy transfer provides a distance-sensitive optical readout. Spectral overlap and fluorophore orientation matter alongside distance. |
| Single-molecule FRET (smFRET) | Measures FRET from individual molecules, revealing distributions and dynamics that ensemble averaging can obscure. It uses the same energy-transfer mechanism as FRET. |
| Fluorescence microscopy | An epi-fluorescence optical path illustrates excitation, wavelength selection, fluorescence collection and photodetection. |
| Diffraction limit | A point emitter produces a finite point spread function (PSF). The teaching example gives a lateral Rayleigh separation of approximately 240 nm for 550 nm emission and NA = 1.4. |
| Single-molecule localization microscopy (SMLM) | Sparse emitters are localized over many frames and their estimated positions form a reconstructed image. Localization precision and image resolution are different quantities. |
| Super-resolution imaging | SMLM is compared briefly with stimulated emission depletion (STED), which suppresses peripheral fluorescence to reduce the effective emitting region. |

Under the Förster model,

$$E = \frac{1}{1+(r/R_0)^6}.$$

Here, *r* is the donor–acceptor fluorophore separation and *R₀* is the distance at which the modeled efficiency is 50%. The approximately 2–8 nm range discussed in the slides is a typical sensitivity range, not a universal cutoff. Proximity or a FRET signal alone does not establish direct binding. See [Ha et al. (2024)](https://doi.org/10.1038/s43586-024-00298-3).

The SMLM example in slide 10 cites Lelek et al., Fig. 3b: 60,000 raw frames and an approximately 44 nm Fourier ring correlation (FRC) resolution estimate. FRC assesses agreement between two data subsets across spatial frequencies; this value describes that reconstruction, not single-emitter precision or a fixed SMLM specification.

## Case Study: Maltose-Binding Protein

Slide 7 discusses **MalE** from [Agam et al. (2023)](https://doi.org/10.1038/s41592-023-01807-0). Maltose binding changes its conformation. Two cysteine-pair variants labeled with Alexa Fluor 546 / Alexa Fluor 647 give opposite FRET changes:

| Variant | Labeling sites | Apo: no ligand | Holo: maltose-bound |
| --- | --- | --- | --- |
| MalE-1 | K29C–S352C | 0.49 ± 0.06 | 0.67 ± 0.05 |
| MalE-2 | D87C–A186C | 0.83 ± 0.03 | 0.71 ± 0.05 |

Values are the paper's averages and standard deviations across **16 laboratories** with usable results, not measurements by the presenter. The slide rounds these to 0.49 → 0.67 and 0.83 → 0.71. The cropped histogram is a representative laboratory-1 dataset, distinct from these cross-laboratory statistics.

The lesson is that the same conformational change can produce different signal directions for different labeling geometries. The slide's structures use PDB **1OMP** and **1ANF**; orange residue markers are not dye centers.

## Optical Engineering Perspective

**Biological questions → Optical observables → Measurement → Biological interpretation**

| Biological question | Optical observable | Measurement and interpretation |
| --- | --- | --- |
| Where is a labeled protein? | Fluorescence position / PSF | Microscopy, with labeling specificity and spatial resolution considered |
| Does its environment change? | Fluorescence decay | FLIM, interpreted with suitable controls |
| Does its conformation change? | FRET efficiency | Calibrated donor/acceptor detection and a labeling-dependent distance model |
| How are labels organized spatially? | Individual emitter positions | SMLM acquisition and reconstruction, with drift and sampling considered |

The optical system determines which information can be recovered: excitation wavelength and stability, filters and dichroic separation, objective numerical aperture, and detector quantum efficiency and noise all influence the signal. Lifetime measurements add timing requirements; localization imaging adds photon-budget, background and reconstruction requirements. Signal-to-noise ratio, calibration and controls connect engineering performance to a defensible biological interpretation.

## Presentation Materials

The 12-slide PPTX and the complete Pages speaking script have been reviewed. Public release of the slide files is on hold because the deck contains third-party figure excerpts. The original files have not been edited.

| Intended repository path | Release status |
| --- | --- |
| `slides/Presentation.pptx` | Withheld pending figure-permission review |
| `slides/Presentation.pdf` | Rendered export prepared; withheld pending figure-permission review |
| [Speaking script (Markdown)](notes/Presentation_Notes.md) | Complete text recovered from Pages; available to read |
| [Speaking script (PDF)](notes/Presentation_Notes.pdf) | Four pages; re-typeset from the complete Pages text and checked |

The notes PDF preserves the script text, timing suggestions and pointing prompts; it does not reproduce the original Pages layout. Slide download links will be added after clearance. See [figure and rights review](references/Rights_Review.md).

## References

The six papers cited in the original deck are listed with DOI links in [References.md](references/References.md):

- Lichtman & Conchello (2005): fluorescence microscopy.
- Torrado et al. (2024): fluorescence lifetime imaging microscopy.
- Ha et al. (2024): single-molecule FRET.
- Agam et al. (2023): MalE case study and smFRET benchmarking.
- Lelek et al. (2021): SMLM principles and the microtubule example.
- Schermelleh et al. (2019): super-resolution methods and STED context.

## Project Information

| Field | Details |
| --- | --- |
| Author / presenter | 卞恺 |
| Institution | Jiangnan University |
| Major | Optoelectronic Information Science and Engineering |
| Course | Introduction to Biomacromolecular Science |
| Presentation date | October 20, 2026 |

The final slide contains unfinished group-contribution fields. Individual preparation roles and any additional contributors remain to be confirmed; this repository does not assign all preparation work to the presenter.

## 中文简介

本项目是江南大学《生物大分子科学导论》课程的本科文献汇报，从光电信息科学与工程视角，梳理荧光标记、寿命成像、FRET及单分子定位成像如何提供蛋白质位置、构象和空间组织信息。MalE与微管图像均为文献实例，不是本人测量或重建的结果。项目用于记录文献学习和课堂汇报，原始幻灯片的公开发布仍待图片版权与成员分工确认。
