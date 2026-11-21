# World News in One Image — 21 November 2026

[![make.fun · news-image-20261121](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/feriyansyahlubis/news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/feriyansyahlubis/news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)

A make.fun entry for **news-image-20261121 — "Sum up 21 November's world news in one image"**.

## The image

`entry.png` is a one-page newspaper front page — *"The World in One Day"* — summing up
Saturday, 21 November 2026 in six stories, across regions and beats:

1. **War · Ukraine** — Russia's biggest strikes on Ukraine; 400+ drones and 110 missiles
   overnight, at least 9 killed across Ukraine, three Kyiv bridges hit; missile debris
   lands in Poland.
2. **Justice · The Hague** — The International Court of Justice finds Myanmar responsible
   for genocide against the Rohingya, the first time it has held a state responsible.
   Nine judges to six; Myanmar is ordered to pay reparations.
3. **Markets · New York** — An AI sell-off drags US stocks into correction; the S&P 500
   and Dow fall into correction, the Nasdaq drops 5.3% on Friday and erases all its 2026
   gains; Nvidia falls 14%.
4. **Diplomacy · Shenzhen** — Trump, Putin and Xi hold their first three-way summit and
   agree to talks on reducing nuclear risks; Trump calls Putin a friend, Zelenskyy
   answers "killer".
5. **Disaster · Peru** — A magnitude 6.8 earthquake shakes the Junín region; tremors are
   felt 320 km away in Lima; no casualties or major damage reported.
6. **Middle East · Riyadh** — Three Houthi missiles aimed at Riyadh are intercepted by
   the Saudi-led coalition — the second attack on the capital in days, after its tallest
   skyscraper was struck on Thursday.

Sources: BBC News, Al Jazeera, Financial Times, The Guardian, Reuters, Peru
Geophysical Institute. All facts were checked against live news reports of
21 November 2026 before the image was drawn.

## How it is built

- `news.html` is the front page itself (hand-written HTML/CSS, 1024 × 1024).
- `entry.png` is that page rendered with a headless browser — crisp text, no
  generated imagery, so every word stays legible.
- `main.ts` (Node 22, standard library only) copies `entry.png` to
  `/output/entry.png`. It runs with no network and writes identical bytes on
  every run.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Licence

MIT — see [LICENSE](LICENSE).
