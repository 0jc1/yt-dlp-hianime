This is a extractor plugin for [yt-dlp](https://github.com/yt-dlp/yt-dlp) that enables downloading content from [HiAnime](https://hianime.to/).
It supports playlist as well as single episodes.

## Installation
If you are using python, you can run the following command to install this plugin:
```bash
python -m pip install -U https://github.com/pratikpatel8982/yt-dlp-hianime/archive/master.zip
```
You can view [Plugin Installation Guide](https://github.com/yt-dlp/yt-dlp?tab=readme-ov-file#installing-plugins)

## Usage
This plugin will be invoked automatically when it detects compatible url.

### List all formats
```
yt-dlp -F [URL]
```
### Subbed (Japanese Audio) with English Subtitles
```
yt-dlp -f b[format_id*=sub] --write-subs --sub-lang en --convert-subs srt [URL]
```
### Dubbed (English Audio) with English Subtitles
```
yt-dlp -f b[format_id*=dub] --write-subs --sub-lang en --convert-subs srt [URL]
```

## Requirements

Python 3.11+ and requests

Recommended to use with yt-dlp python package instead of binaries.
