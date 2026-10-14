# Strand by Strand: oligonucleotides on a single quadrupole

**Live site:** https://kogason2010.github.io/lcms-2050-oligos/

A scroll-driven three.js walk through four Shimadzu application notes on confirming synthetic
oligonucleotides with the LCMS-2050 single quadrupole mass spectrometer:

1. **SSI 02-SSI-LCMS-173** (Jayasundara, Johnson, Nov 2024): ion-source optimization to strip HFIP adducts under ion-pair LC.
2. **01-00766-EN** (Fujisaki, Suzuki, Sep 2024): method development for a 20-mer and five impurities with LabSolutions MD.
3. **01-01180-EN** (Nakazono, May 2026): ion-pair-free reversed-phase LC/MS of a patisiran-based siRNA.
4. **01-01238-EN** (Hayakawa, Kato, Uchiyama, Jul 2026): HILIC impurity analysis of a mipomersen-based 20-mer.

> Independent, unofficial project. Not affiliated with, sponsored or endorsed by Shimadzu Corporation.

- **Single file:** `index.html` (three.js r128 and its bloom passes load from cdnjs and jsDelivr).
- **Demo mode:** press *Play demo* or the D key for a guided scroll of about two minutes.
- **Interactive:** a charge-state ladder built from published peaks, a Qarray voltage sweep, and the 24-run screening grid.
- Companion sites: https://kogason2010.github.io/nexera-uc-epsa/ · https://kogason2010.github.io/nexera-ic/ · https://kogason2010.github.io/nexera-ic-applications/

## Data and accuracy

Taken from the notes: all tables (optimized source settings, deconvolution results, top-10 evaluation values,
resolutions at the optimum, estimated and theoretical molecular weights, HILIC linearity), m/z values for the
charge ladders (HILIC n-3(5′) and n-1(5′), siRNA sense strand), conditions, and retention times for HILIC
(8.432, 8.956, 9.300 min).

Approximate (read from figures): Qarray bar heights (SSI Fig. 1), peak positions and heights of the redrawn
chromatograms (01-00766 Fig. 13, 01-01180 Fig. 3, 01-01238 Fig. 1 heights).

Calculated: the per-rung neutral mass in the charge ladder, |z| × m/z ± |z| × 1.00728. Rungs disagree by up to
about 2 Da because single-quadrupole peaks are unit resolution; the deconvoluted values shown are the software's.

Illustrative: all 3D geometry (strands, adducts, duplex, columns) and the speed of strands through the columns,
which is scaled to the published retention times.

Notes on the sources: the SSI note's text gives desolvation line and desolvation temperatures as 500 °C and
250 °C, but its Table 3 gives 250 °C (line) and 500 °C (desolvation); the site follows the table. The 01-01180
siRNA note defines "m" as 5-methyl; the site does not restate the modifications.
