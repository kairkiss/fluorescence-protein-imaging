# Figure attribution and public-release review

Reviewed October 20, 2026. This is a record of source checks and unresolved release conditions, not a claim of permission or a legal determination.

## Archive status update — October 20, 2026

After reading the initial review, the repository owner explicitly requested public archival of the complete, unchanged original PPTX. It is now included as `slides/Presentation.pptx`. The initial findings below are retained as the review record; the owner's publication instruction is not evidence of permission from third-party rightsholders. All original citations and unfinished contribution fields remain unchanged. No replacement illustrations or blanket license have been added.

## Initial review: original slide files placed on hold

| Material | Evidence in the supplied deck | Release consideration |
| --- | --- | --- |
| Slide 7: MalE histograms | Cropped parts of Agam et al., Fig. 1c; source and figure number appear on the slide | The article carries [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), subject to credit-line exclusions. Before release, add a companion notice naming authors, DOI, license and the cropping/rearrangement. Check the exact figure credit lines. |
| Slide 10: microtubule comparison | Raster excerpt from Lelek et al., Fig. 3b; caption credits the paper | The [publisher rights section](https://www.nature.com/articles/s43586-021-00038-x#rightslink) states exclusive rights. No permission for this repository's republication has been established. This is the principal release blocker. |
| Slide 7: structure projections | PDB 1OMP / 1ANF, with residue markers; distinct from the paper histogram | Keep the PDB identifiers and describe the added residue markers. Their positions are not fluorophore-center positions. |
| Other slides: diagrams and explanatory graphics | Predominantly editable shapes with “Adapted from” source lines | Attribution is present, but it is not a license. Independent explanatory diagrams and close adaptations require different assessments; provenance and any close figure adaptations should be confirmed before releasing the whole deck. |

The Agam article's license can be checked in the [institutionally hosted published PDF](https://documentserver.uhasselt.be/bitstream/1942/40281/1/Reliability%20and%20accuracy%20of%20single-molecule%20FRET%20studies%20for%20characterization%20of%20structural%20dynamics%20and%20distances%20in%20proteins.pdf), printed page 535. Open access is not a blanket license for every third-party component.

The Pages script contains speaking text and slide-pointing prompts, with no embedded paper-figure media in its package. Its scientific examples remain attributed to the cited literature. Its final section explicitly leaves member contributions unresolved.

## Concrete options for the owner

1. Publish the text documentation first and keep the original deck offline until reuse permission is documented.
2. Obtain permission covering public GitHub distribution of the Lelek figure excerpt, and check any other adapted figures before uploading the unchanged deck.
3. Authorize a separate public edition using independently created illustrations or appropriately licensed alternatives, with accurate attribution. Preserve the original PPTX separately; do not label an altered edition as the unchanged original.

No original figures have been removed, replaced or edited during this review. A public branch or pull request is also public; it is not a private holding area for restricted figures.

## Licensing scope

No repository-wide LICENSE has been added. Public availability does not make the materials public domain, and the presenter cannot grant rights owned by article authors, publishers or other rightsholders. Any future license for original project text must explicitly exclude third-party material and preserve its own applicable terms.

## Contribution confirmation

Slide 12 contains `卞恺｜__________`, `成员2｜__________`, and `成员3｜__________`. Confirm the actual participants and roles before publishing a revised contribution statement. Neither blank names nor contribution roles have been invented.
