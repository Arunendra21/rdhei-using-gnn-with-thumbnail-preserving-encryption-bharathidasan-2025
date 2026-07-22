# RDHEI using Graph Neural Networks & Thumbnail-Preserving Encryption (Bharathidasan 2025)

This repo is my reproduction of RDHEI using Graph Neural Networks & Thumbnail-Preserving Encryption, from S. Bharathidasan, V. Tamil Selvi, V. Sathiya, Francis H. Shajin, published in Signal, Image and Video Processing, vol. 19, 2025.

It leans on a graph neural network together with thumbnail preserving encryption, so the protected image still looks like the original at a glance.

This one depends on a trained network, real 3D or HDR data, or a full cloud system that I could not rebuild faithfully here. So the repo carries a complete report of the method, an honest account of what blocks a full reproduction, and a small demo of the central idea so the mechanism is not just described but shown.

## Running it

Everything runs with plain Python and a handful of common libraries. From this folder:

```bash
cd source_code
python3 run_experiment.py       # runs the method, writes metrics and figures
python3 build_deliverables.py   # rebuilds the IEEE report and the slides
```

You need numpy, scipy, matplotlib, pillow, python-docx and python-pptx. Install them with `pip install numpy scipy matplotlib pillow python-docx python-pptx`. The report is exported to PDF with headless LibreOffice, so that has to be on the machine if you want the PDF rebuilt.

## What sits in this folder

```
(the original paper stays on my machine and is not republished here, to respect its copyright)
ieee_report.docx/.pdf  my IEEE format reproduction report
presentation.pptx      a short summary deck
source_code/           the scripts that do the actual work
outputs/               metrics.json and the raw numbers behind the report
figures/               the plots and images the code produces
processing_notes.md    what was reproduced, what was not, and the caveats
```

## A note on honesty

Nothing in the tables or plots was copied from the paper. Anything marked as reported, and only that, is quoted from the original for comparison. Everything else is computed here. Where the exact image set or an unstated hyperparameter differs from the paper, the absolute figures can move a little, but the behaviour and the reversibility hold. The specifics for this paper are in `processing_notes.md`.
