# What Readers Love

**What makes a book popular on Goodreads?**

Is reader attention simply a numbers game — more books, more ratings? Or do popularity, reader disagreement, genre, and author consistency tell a more complicated story?

This project explores those questions using Goodreads book and review data covering **13,525 books and more than 1.14 million reviews**.

## Questions I'm Exploring

- Which books attract the most reader attention?
- Does publishing more books translate into greater reach for an author?
- Which books generate the strongest disagreement among readers?
- Which genres have the strongest typical engagement?
- Do highly-rated authors sustain strong ratings across their published works?

## The Investigation

Rather than treating ratings as a single measure of success, the analysis looks at reader engagement from several angles:

**Popularity** — Which books dominate the Goodreads ratings landscape?

**Author reach** — Does catalogue size explain how many readers an author's books reach?

**Reader disagreement** — Can a book be highly popular while also dividing its readers?

**Genre engagement** — Do smaller genres sometimes outperform larger categories on a per-book basis?

**Reception over time** — Do authors with consistently high ratings maintain that reception throughout their catalogues?

## What I Found

The analysis uncovered several patterns that challenged some of the initial assumptions — including a surprisingly weak relationship between catalogue size and total ratings, substantial differences in engagement across genres, and cases where enormous popularity coexists with strong reader disagreement.

The full findings are presented in the **[Goodreads Data Story](docs/goodreads_data_story.md)**.

For the complete analysis, methodology, visualizations, and supporting calculations, see the **[EDA notebook](notebooks/goodreads_eda.ipynb)**.

## Project Structure

```text
what-readers-love/
├── data/
│   ├── goodreads_works.csv
│   ├── goodreads_reviews.csv
│   └── goodreads_data_dictionary.csv
├── notebooks/
│   └── goodreads_eda.ipynb
├── docs/
│   └── goodreads_data_story.md
├── README.md
└── requirements.txt
```

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Git / GitHub

## Dataset

The project uses the Goodreads books & reviews dataset, containing book-level metadata and a large collection of Goodreads reader reviews. The analysis focuses primarily on the book-level `works` data, while the `reviews` data is used during data-quality and dataset exploration.

CSVs are not committed (`goodreads_reviews.csv` alone is ~880MB, over GitHub's limit). To reproduce, download the dataset and place these files in `data/`:
- `goodreads_data_dictionary.csv`
- `goodreads_works.csv`
- `goodreads_reviews.csv`

---

**Start with the [EDA notebook](notebooks/goodreads_eda.ipynb) to follow the investigation, or read the [data story](docs/goodreads_data_story.md) for the conclusions.**
