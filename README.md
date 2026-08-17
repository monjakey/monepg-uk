# mon's EPG 🇬🇧

A curated United Kingdom programme guide, shared
through [EPGenius](https://epgenius.org/).

This repository hosts the two files the playlist needs, plus its artwork.
It contains no credentials and no streams — an EPGenius playlist is a template,
and it does nothing until you supply your own provider credentials.

| File | What it is |
|---|---|
| `monepg-uk.m3u` | the playlist template |
| `monepg-uk.xml.gz` | the programme guide (XMLTV, gzipped) |
| `logos/` | channel artwork referenced by both files |
| `assets/` | playlist branding |

## What's in it

**Around 1,200 channels, United Kingdom only.** The exact count moves daily —
event channels are published only while they carry something, so a slot with no
fixture is hidden rather than shipped empty.

- **UK TV Guide** — terrestrials, news, entertainment, factual, kids, sport,
  shopping, then nations and regions.
- **Sky Sports**, including the Sky Sports+ event slots named with the real
  fixture rather than a slot number, and an `Ended:` card afterwards so a slot is
  never blank.
- **Sky Entertainment** and **TNT Sports**
- **Football club channels** with crests — Premier League, Championship, League
  One, League Two, National League, La Liga, Serie A, SPFL.
- **Formula 1** — broadcast feeds plus 22 driver onboards, each with that
  driver's headshot, on a session schedule.
- **Tennis TV** — court feeds with a liveness guide refreshed five times a day.
- **NBA** — League Pass, team channels and the Replay block.
- **ITVX**, **DAZN**, **Premier Sports**.
- **UK Radio, ~700 stations** — credential-free public streams, so they work for
  everyone.

## Guide quality

The guide is the point of this list.

- **First-party Sky data on 126 channels**, taken from Sky's own public API
  rather than a scraped third party.
- **No blank guides.** A channel that cannot get a real guide is left out rather
  than shipped empty.
- **No `+1` contamination** — no channel is bound to its own timeshift feed.
- **Rebrands tracked by schedule, not by name** — Sky retired several brands its
  streams are still labelled with.

## Using it

Pick this playlist on [epgenius.org](https://epgenius.org/), supply your own credentials, and EPGenius builds your copy. The guide updates
automatically — you do not need to re-import it.

## Notes

- Radio channels are public streams and carry `tvg-type="ignore"`, so EPGenius
  passes them through without credential substitution.
- Channel ids are stable across renames, so your guide bindings survive updates.
