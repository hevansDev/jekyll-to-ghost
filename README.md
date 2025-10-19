# Jekyll to Ghost Migration Tool

Convert Jekyll blog posts to Ghost CMS format.

## Usage

```bash
python3 jekyll_to_ghost.py /path/to/_posts output.json
```

## What it does

- Converts markdown posts to Ghost JSON
- Extracts featured images from front matter
- Preserves tags and canonical URLs
- Fixes image paths automatically

## After running

1. Copy images to Ghost i.e.

```bash
   cp /path/to/assets/images/. ghost/content/images/
```

2. Import JSON in Ghost Admin → Settings → Labs → Import content

3. Set Ghost site URL in Settings → General

## Requirements

- Python 3.6+
- Jekyll posts with YAML front matter