# data-science-notebooks

Jupyter notebooks for exploratory data analysis, statistical exploration,
and reproducible mini-studies.

Planned notebooks:
- `01_pandas_fundamentals.ipynb`
- `02_eda_template.ipynb`
- `03_statistical_tests.ipynb`
- `04_data_visualization_with_seaborn.ipynb`

Each notebook documents the dataset, the questions explored, the methods
applied, and the conclusions drawn.

## Notebook conventions

To keep the repo reviewable, every notebook follows the same skeleton:

1. **Question** — one sentence stating what the notebook answers.
2. **Data** — source, shape, dtypes, and any cleaning notes.
3. **Method** — what was done and *why this approach* over alternatives.
4. **Result** — the headline finding, ideally in one chart and one
   number.
5. **Caveats** — what the analysis does not say.

**Next pickup:** `01_pandas_fundamentals.ipynb` — a working reference
notebook (groupby, merge, reshape, time-indexed ops) that later
notebooks can link to instead of re-deriving basics.

---

### Log

- **2026-05-25** — The five-step skeleton (Question / Data / Method /
  Result / Caveats) is non-negotiable: every notebook in this repo must
  open with a one-sentence question and close with one chart + one
  number. If a notebook can't be summarized that way, the question
  isn't sharp enough yet — split it into two notebooks.

- **2026-05-27** -- Pinning a "one notebook = one question" rule in
  practice: when `01_pandas_fundamentals.ipynb` lands, it answers
  *"what's the smallest reusable subset of pandas idioms I need for
  90% of EDA?"* -- not "everything pandas can do." The other 10% lives
  in `02_eda_template.ipynb` where it gets called by name. Same
  separation-of-concerns instinct that makes the DP rolling-window
  trick work: keep state minimal, defer the rest.
