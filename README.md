# Awesome Kurdish Tech

A curated list of Kurdish language tools, datasets, and resources.

## Tools

### Data Collection

- [kurdish_scrapy](https://github.com/cikay/kurdish_scrapy) — Scrapy-based crawler that collects Kurdish text from websites, extracts article content (Trafilatura), and filters by language (FastText) including `kmr_Latn`, `ckb_Arab`, and `diq_Latn`.

### Text Preprocessing

- [kmr_standardizer](https://github.com/cikay/kmr_standardizer) — Regex-based Kurmanji (Kurmancî) text standardizer that applies orthographic rules from *Rêbara Rastnivîsînê* (Weqfa Mezopotamya).
- [Kurdish Language Processing Toolkit (KLPT)](https://github.com/sinaahmadi/klpt) — Kurdish NLP toolkit in Python.

### Language Identification

- [facebook/fasttext-language-identification](https://huggingface.co/facebook/fasttext-language-identification) — fastText language identification model (`lid218e`) for 217 languages (includes Kurdish varieties such as Kurmanji and Sorani).

## Datasets

- [muzaffercky/kurdish-kurmanji-news](https://huggingface.co/datasets/muzaffercky/kurdish-kurmanji-news) — ~271k Kurdish (Kurmanji, Latin script) news articles with `title`, `url`, and `content` columns (train/test splits).
- [kurdish-twitter-data](https://github.com/ftkurt/kurdish-twitter-data) — Kurdish Twitter data for Kurmanji and Sorani.

## Contributing

PRs are welcome. If you add a link, please include a short, concrete description and keep the format:

`- [name](link) — one-line description`
