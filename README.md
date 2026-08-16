# mon's EPG 🇬🇧

A curated United Kingdom playlist and programme guide for **Strong 8K**, shared
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

**1,152 channels, United Kingdom only.**

- **UK TV Guide (94)** — terrestrials, news, entertainment, factual, kids, sport,
  shopping, then nations and regions.
- **Sky Sports (44)**, including the Sky Sports+ event slots named with the real
  fixture rather than a slot number, and an `Ended:` card afterwards so a slot is
  never blank.
- **Sky Entertainment (11)**, **TNT Sports (13)** — every TNT channel carries a
  guide, including Event 10.
- **Football, 182 club channels** with crests — Premier League, Championship,
  League One, League Two, La Liga, Serie A, SPFL.
- **Formula 1 (28)** — broadcast feeds plus 22 driver onboards, each with that
  driver's headshot, on a session schedule.
- **Tennis TV (20)** — court feeds with a liveness guide refreshed five times a day.
- **NBA (59)** — League Pass, team channels and the Replay block.
- **ITVX (16)**, **DAZN (23)**, **Premier Sports (4)**.
- **UK Radio (698)** — credential-free public stations, so they work for everyone.

## Guide quality

The guide is the point of this list.

- **First-party Sky data on 126 channels**, taken from Sky's own public API
  rather than a scraped third party.
- **No blank guides.** A channel that cannot get a real guide is left out rather
  than shipped empty.
- **No `+1` contamination** — no channel is bound to its own timeshift feed.
- **No wrong-country schedules** — no German listings on UK kids channels, no US
  schedules on UK channels.
- **Rebrands tracked by schedule, not by name** — Sky retired several brands its
  streams are still labelled with.
- **Every stream measured** rather than trusted: provider "4K" labels are
  frequently wrong, and every pick here was checked with `ffprobe`.

## Using it

Pick this playlist on [epgenius.org](https://epgenius.org/), supply your own
Strong 8K credentials, and EPGenius builds your copy. The guide updates
automatically — you do not need to re-import it.

## Notes

- Radio channels are public streams and carry `tvg-type="ignore"`, so EPGenius
  passes them through without credential substitution.
- Channel ids are stable across renames, so your guide bindings survive updates.
