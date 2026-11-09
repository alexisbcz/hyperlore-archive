# Hyperlore archive

The content behind [Hyperlore](https://hyperlore-441.netlify.app), the sourced history of startups: renames, logos, funding rounds, launches and quotes, collected by agents from primary sources. Every fact links to where it was found.

The code (the agents' CLI, their methods and the website) lives in [alexisbcz/hyperlore](https://github.com/alexisbcz/hyperlore). This repo holds what they collected, as plain files:

| Path | What |
| --- | --- |
| `archive.json` | The whole archive: every event, quote, source, entity (companies, people, investors, places) and overview page. Each event cites its sources by URL, with the verbatim words that support it. |
| `assets/<company>/` | Logos, wordmarks, icons and screenshots through the years, as the site serves them. Each one is an `assets` record in `archive.json`, with the snapshot or page it came from. |
| `people/`, `places/` | Portraits and photos, each attributed in the matching entity's `photo` field. |
| `transcripts/` | Timestamped transcripts of founder interviews, talks and podcasts (`[<seconds>s] text`), so quotes link to the exact second. |

Pushing here rebuilds the site.

## Corrections and requests

Open an issue: [request a company](../../issues/new?labels=request&title=Request:%20) or [report a wrong fact](../../issues/new?labels=correction&title=Correction:%20) with a link to the source that shows the right version. The forms on the site pre-fill these.

## Notes

- Logos, photos, quotes and transcripts belong to their owners and are kept here as a cited historical record. Each record names its source.
- Transcripts come from YouTube captions, ScrapeCreators or Whisper. Their metadata was stripped of signed media URLs before publishing.
