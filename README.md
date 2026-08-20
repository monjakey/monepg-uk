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

**Around 1,200 channels, United Kingdom only.**

- **UK TV Guide** — terrestrials, news, entertainment, factual, kids, sport,
  shopping, then nations and regions.
- **Sky Sports**, including the Sky Sports+ event slots.
- **Sky Entertainment** and **TNT Sports**
- **Football club channels** with crests — Premier League, Championship, League
  One, League Two, National League, La Liga, Serie A, SPFL.
- **Formula 1** — broadcast feeds plus 22 driver onboards, each with that
  driver's headshot.
- **Tennis TV** — court feeds.
- **NBA** — League Pass, team channels and the Replay block.
- **ITVX**, **DAZN**, **Premier Sports**.
- **UK Radio, ~700 stations** — credential-free public streams, so they work for
  everyone.

## Guide quality

The guide is the point of this list.

- **Every channel has one.** Nothing here ships with an empty grid, and
  scrolling forward does not run out.
- **Club channels tell you the next fixture.** A team channel reads
  `Upcoming: Home to Bolton, Sat 22 Aug 15:00` — the opposition named the short
  way a supporter would say it, and home or away stated.
- **Event slots name the event**, not the slot, and say `Ended:` once it has
  finished rather than still advertising it as live.
- **Sky channels carry Sky's own data.**
- **The channel list is stable.** Your ordering, favourites and guide bindings
  survive updates.

## Using it

Pick this playlist on [epgenius.org](https://epgenius.org/), supply your own credentials, and EPGenius builds your copy. The guide updates
automatically — you do not need to re-import it.

## Notes

- Radio channels are public streams and carry `tvg-type="ignore"`, so EPGenius
  passes them through without credential substitution.
- Channel ids are stable across renames, so your guide bindings survive updates.

## Credits

This playlist is assembled from other people's work. Nothing here would exist
without them.

**The software it runs on**

- **[Dispatcharr](https://github.com/Dispatcharr/Dispatcharr)** — the channel
  and guide platform the whole service is built on. Licensed AGPL-3.0.
- **[Teamarr](https://github.com/Pharaoh-Labs/teamarr)** by Pharaoh Labs —
  generates the per-team fixture guide behind every football and NBA club
  channel in this list. The club channels are its work, not ours.

**Programme data**

- **[epg.guru](https://epg.guru/)** and its maintainers — the guide source
  behind most of the entertainment, factual and kids channels here.
- **Sky** — the first-party public EPG API, used for the Sky and Sky Sports
  channels and for the Sky Sports+ event slots.
- **ESPN** — fixture and session data for Formula 1, the football club channels
  and the National League slots.

**Artwork**

- **[K-yzu/Logos](https://github.com/K-yzu/Logos)** — television and radio
  channel logos. The great majority of the tiles in `logos/` come from here.
- **[football-logos.cc](https://football-logos.cc/)** — football club crests.

**Distribution**

- **[EPGenius](https://epgenius.org/)** — hosts the playlist, republishes the
  guide, and handles credential substitution so this repository never has to
  hold any.

Channel logos and club crests remain the property of their respective
broadcasters and clubs, and are used here for identification only. If you
maintain something credited above and would like the attribution changed — or
removed — open an issue and it will be done.
