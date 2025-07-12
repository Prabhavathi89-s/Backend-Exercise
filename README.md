# PubMed Paper Fetcher

Fetch PubMed research papers with at least one author from pharmaceutical/biotech companies.

## Features

- Full PubMed query support.
- Filters papers with at least one non-academic affiliation.
- Outputs results to console or CSV.

## Installation

```bash
git clone https://github.com/yourusername/pubmed-paper-fetcher.git
cd pubmed-paper-fetcher
poetry install
```

## Usage

```bash
poetry run get-papers-list "cancer immunotherapy" -f results.csv
```

Options:

- `-d, --debug`: Enable debug mode
- `-f, --file <filename>`: Save results to CSV

## Publishing (Test PyPI)

```bash
poetry config repositories.testpypi https://test.pypi.org/legacy/
poetry publish -r testpypi --build
```

## Tools Used

- [PubMed API](https://www.ncbi.nlm.nih.gov/home/develop/api/)
- [Poetry](https://python-poetry.org/)
- [Requests](https://pypi.org/project/requests/)
