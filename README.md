# Awesome Kurdish Tech

A curated list of Kurdish language AI models, datasets and packages

## AI Models

### Language Identification

- [cis-lmu/glotlid](https://huggingface.co/cis-lmu/glotlid) — GlotLID language identification model that distinguishes Kurdish varieties including Zaza language and Kurmanji more correctly.
- [facebook/fasttext-language-identification](https://huggingface.co/facebook/fasttext-language-identification) — fastText language identification model (`lid218e`) for 217 languages; useful for broad filtering, but it does not reliably distinguish Zaza language and Kurmanji.

### Speech

#### Text To Speech(TTS)

- [facebook/mms-tts-kmr-script_latin](https://huggingface.co/facebook/mms-tts-kmr-script_latin) — Meta MMS text-to-speech model for Kurmanji (`kmr`, Latin script).

#### Forced Alignment

- [MahmoudAshraf/mms-300m-1130-forced-aligner](https://huggingface.co/MahmoudAshraf/mms-300m-1130-forced-aligner) — Forced aligner based on Meta MMS that gives word level timestamps and helps split long audio when preparing TTS and ASR datasets. It supports Kurdish through MMS language codes like Central Kurdish Sorani ckb and Kurmanji kmr-script_latin kmr-script_arabic kmr-script_cyrillic.

## Datasets

### Text datasets

- [HuggingFaceFW/fineweb-2](https://huggingface.co/datasets/HuggingFaceFW/fineweb-2) — Multilingual Common Crawl pretraining corpus with Kurdish subsets: Central Kurdish (`ckb_Arab`), Kurmanji (`kmr_Latn`, `kmr_Cyrl`), Zazaki (`diq_Latn`), Kirmanjki (`kiu_Latn`), Southern Kurdish (`sdh_Arab`), and Laki (`lki_Arab`).
- [muzaffercky/kurdish-kurmanji-news](https://huggingface.co/datasets/muzaffercky/kurdish-kurmanji-news) — ~271k Kurdish (Kurmanji, Latin script) news articles with `title`, `url`, and `content` columns (train/test splits).
- [muzaffercky/kurdish-kurmanji-theses](https://huggingface.co/datasets/muzaffercky/kurdish-kurmanji-theses) — 389 Kurmanji (Latin script) academic theses extracted from the Turkish national thesis repository (YÖK), totalling 57.6 MB; non-Kurdish paragraphs filtered via GlotLID v3 (≥0.7 confidence); includes thesis ID, title, URL, word count, and cleaned text.
- [kurdish-twitter-data](https://github.com/ftkurt/kurdish-twitter-data) — Kurdish Twitter data for Kurmanji and Sorani.

### Speech datasets

## Packages

### Data Collectors

- [kurdish_scrapy](https://github.com/cikay/kurdish_scrapy) — Scrapy-based crawler that collects Kurdish text from websites, extracts article content (Trafilatura), and filters by language (FastText) including `kmr_Latn`, `ckb_Arab`, and `diq_Latn` or any other language.
- [kurdish-kurmanji-thesis](https://github.com/cikay/kurdish-kurmanji-thesis) — Pipeline that scrapes Kurmanji theses from YÖK Ulusal Tez Merkezi, extracts and normalizes text via PyMuPDF, filters to Kurmanji-only content using GlotLID v3, and publishes to Hugging Face.

### Text Preprocessing

- [kmr_standardizer](https://github.com/cikay/kmr_standardizer) — Regex-based Kurmanji (Kurmancî) text standardizer that applies orthographic rules from *Rêbara Rastnivîsînê* (Weqfa Mezopotamya).
- [Kurdish Language Processing Toolkit (KLPT)](https://github.com/sinaahmadi/klpt) — Kurdish NLP toolkit in Python.

## Contributing

PRs are welcome. If you add a link, please include a short, concrete description and keep the format:

`- [name](link) — one-line description`
