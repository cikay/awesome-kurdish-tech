# Awesome Kurdish Tech

A curated list of Kurdish language AI models, datasets and packages

## AI Models

### Language Identification

- [facebook/fasttext-language-identification](https://huggingface.co/facebook/fasttext-language-identification) — fastText language identification model (`lid218e`) for 217 languages (includes Kurdish varieties such as Kurmanji and Sorani).

### Speech

#### Text To Speech(TTS)

- [facebook/mms-tts-kmr-script_latin](https://huggingface.co/facebook/mms-tts-kmr-script_latin) — Meta MMS text-to-speech model for Kurmanji (`kmr`, Latin script).

#### Forced Alignment

- [MahmoudAshraf/mms-300m-1130-forced-aligner](https://huggingface.co/MahmoudAshraf/mms-300m-1130-forced-aligner) — Forced aligner based on Meta MMS that gives word level timestamps and helps split long audio when preparing TTS and ASR datasets. It supports Kurdish through MMS language codes like Central Kurdish Sorani ckb and Kurmanji kmr-script_latin kmr-script_arabic kmr-script_cyrillic.

## Datasets

### Text datasets

- [muzaffercky/kurdish-kurmanji-news](https://huggingface.co/datasets/muzaffercky/kurdish-kurmanji-news) — ~271k Kurdish (Kurmanji, Latin script) news articles with `title`, `url`, and `content` columns (train/test splits).
- [kurdish-twitter-data](https://github.com/ftkurt/kurdish-twitter-data) — Kurdish Twitter data for Kurmanji and Sorani.

### Speech datasets

- [azadiya-welat-kurdish-kurmanji-voice](https://huggingface.co/datasets/muzaffercky/azadiya-welat-kurdish-kurmanji-voice) — Paired Kurmanji audio-text corpus with 15,284 segments (25.9h) of 16 kHz mono WAV from Azadiya Welat news readings, aligned to Latin script transcripts for TTS and ASR fine-tuning.

## Packages

### Data Collectors

- [kurdish_scrapy](https://github.com/cikay/kurdish_scrapy) — Scrapy-based crawler that collects Kurdish text from websites, extracts article content (Trafilatura), and filters by language (FastText) including `kmr_Latn`, `ckb_Arab`, and `diq_Latn` or any other language.

### Text Preprocessing

- [kmr_standardizer](https://github.com/cikay/kmr_standardizer) — Regex-based Kurmanji (Kurmancî) text standardizer that applies orthographic rules from *Rêbara Rastnivîsînê* (Weqfa Mezopotamya).
- [Kurdish Language Processing Toolkit (KLPT)](https://github.com/sinaahmadi/klpt) — Kurdish NLP toolkit in Python.

## Contributing

PRs are welcome. If you add a link, please include a short, concrete description and keep the format:

`- [name](link) — one-line description`
