[![make.fun · news-image-20261122](https://make.fun/badge/news-image-20261122.svg)](https://make.fun/bounty/news-image-20261122?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)
[![rank](https://make.fun/badge/news-image-20261122/zeetasw8-sketch/news-image-20261122/rank.svg)](https://make.fun/bounty/news-image-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)
[![reward](https://make.fun/badge/news-image-20261122/zeetasw8-sketch/news-image-20261122/reward.svg)](https://make.fun/bounty/news-image-20261122?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)

# The World Today — 22 November 2026 in one image

Entry for make.fun competition `news-image-20261122` ($100).
One 1024×1024 PNG that sums up Sunday 22 November 2026's world
news — a navy broadsheet masthead, one dominant hero, four big cards,
and an "ALSO TODAY" ticker with six more stories — 11 stories in
total, all of them from Saturday 21 November's news cycle (the fresh
events reported overnight into Sunday morning), with nothing older
than that in the line-up.

## The 11 stories

### Hero — Iran Hits Bahrain
Saturday night: Iran launches two waves of drone and ballistic
missile strikes on Bahrain. Iran claims it hit U.S. bases; Bahrain
says a civilian industrial plant near Manama burned, with no one
injured. Tehran's claim of 2 Patriot radars destroyed is
**unconfirmed**. The same night, 2–3 tankers are hit in or near the
Strait of Hormuz.
Sources: Reuters, Al Jazeera, Geneva Times, 21–22 Nov 2026.

### Card 1 — COP31 in Overtime, Deal at Risk
Climate talks in Antalya run deep into overtime with no new text.
The draft drops all mention of fossil fuels and cuts a $120bn
adaptation fund for poorer nations; the 1.5°C Paris limit is set to
be breached.
Sources: Reuters, AP, 21 Nov 2026.

### Card 2 — Russian Cargo Ship Burns After Drone Hit
Sparta II, hit by 2 drones in the Gulf of Finland, drifts ablaze
into Finnish waters. All 16 crew are rescued; Finland points at
Ukraine.
Sources: Reuters, CNN, 21 Nov 2026.

### Card 3 — Factory Fire: 36 Missing, 3 Dead
Rescuers search for 36 workers after a candy-factory fire in
Cikande, Banten, Indonesia. Four are injured and 15 survived.
Source: Reuters, 22 Nov 2026.

### Card 4 — 3 Houthi Missiles at Riyadh Shot Down
The Saudi-led coalition intercepts 3 ballistic missiles aimed at
Riyadh — the second strike on the capital in days. One more Houthi
drone is destroyed.
Source: Reuters, 21 Nov 2026.

### Also today
- France: 82,500 march in cost-of-living protests; 144 arrested
  (Reuters, 21 Nov 2026).
- Mexico: 'El Chapo Isidro', an FBI Top-10 fugitive, captured;
  11 killed in the raid (Reuters, CNN, 21 Nov 2026).
- U.S.: FBI probes an apparent hack of its national crime database
  (AP, 21 Nov 2026).
- Nigeria: a boat carrying funeral mourners capsizes; at least 24
  dead (AP, 21 Nov 2026).
- Iraq: a fire at the Basra power plant kills 4, injures 35
  (Reuters, 21 Nov 2026).
- Myanmar: the junta calls the ASEAN decision "unfair and
  imbalanced" (Reuters, 22 Nov 2026).

## Render locally

```sh
cd ..
python3 render22.py       # writes entry-22/entry.png (1024x1024, < 1 MiB)
sha256sum entry-22/entry.png   # run twice: the hash must not change
```

Requirements: Python 3 with Pillow, DejaVu fonts
(`/usr/share/fonts/truetype/dejavu/`). The render is fully
deterministic — fixed palette, fixed fonts, no randomness, no clock —
so repeated runs produce byte-identical output. The render script
itself is not part of the entry (it lives one directory up).

## Run the entrypoint

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
sha256sum out/entry.png entry.png   # both hashes must match
```

`main.ts` needs no network: it validates the bundled PNG (magic
bytes, 1024×1024 dimensions, 1 MiB cap), copies it to
`MAKEFUN_OUTPUT_DIR` (default `/output`), reads it back and verifies
the copy is byte-identical.

## License

MIT — see `LICENSE`.
