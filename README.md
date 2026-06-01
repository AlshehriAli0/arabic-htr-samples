# Arabic Handwriting Line Samples

A small evaluation set of real handwritten Arabic **text-line** images with ground-truth transcriptions.

```
arabic-htr-samples/
 ├─ images/      50 handwritten Arabic line images (.tif, loose files)
 └─ labels.csv   filename,ground_truth_text  (logical-order Arabic, exactly as written)
```

## Source

Images are drawn from the **KHATT** and **IFN/ENIT** Arabic handwriting datasets — handwritten
line and word images (`*.tif`), each paired with its original transcription. Samples are spread
across many writers for diversity.

## labels.csv

- UTF-8, comma-separated, with a header row.
- `filename` — image file name under `images/`.
- `ground_truth_text` — the transcription in **logical (reading) order**, exactly as written
  (original diacritics/punctuation kept). Fields containing commas are quoted per RFC 4180.
- Images whose source transcription was empty were skipped.

## Counts

- 50 images / 50 labeled rows.

## Usage

These samples are provided for research and evaluation. The underlying KHATT and IFN/ENIT
datasets are subject to their respective original terms; please consult each dataset's license
before redistribution.
