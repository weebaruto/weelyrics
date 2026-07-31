# weelyrics

This repo is a **metadata-only** song catalogue: title, artist, year, tags, a
personal note, and a link to the full lyrics on Genius. **Do not add lyric
text.** The full lyrics are displayed by Genius (a licensed platform) via the
`geniusUrl` link — this site never reproduces them. That's what keeps the
catalogue clear of copyright issues.

Each song is one flat `.md` file whose entire content is frontmatter (no body):

```markdown
---
title: A Song for Life
artist: Ralph McTell
year: 1971
tags: [folk, comfort]
geniusUrl: https://genius.com/Ralph-mctell-a-song-for-life-lyrics
note: The one that always brings me back to myself.
---
```

The filename (slug) becomes the song's id and URL segment. If a `geniusUrl` is
missing, the song page simply omits the outbound button.
