# news-image-20261117

[![make.fun · news-image-20261117](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![rank](https://make.fun/badge/news-image-20261117/garrs27/news-image-20261117/rank.svg)](https://make.fun/bounty/news-image-20261117/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![reward](https://make.fun/badge/news-image-20261117/garrs27/news-image-20261117/reward.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)

**The World in One Image — Tuesday, 17 November 2026.** A single front-page
image that sums up the day's world news: Trump, Xi and Putin converging on
Shenzhen for a first three-way summit, the US strike on Iran's Qeshm Island
as a tanker burned in Hormuz, Ukraine striking the Crimean Bridge again,
Quad leaders unveiling critical-minerals pacts in Manila, Washington
tightening AI chip rules, Wall Street falling, and the US losing its
measles elimination status.

![The world in one image, 17 November 2026](entry.png)

`entry.png` is the entry image: 1024x1024, under 1 MiB, with the date in
the masthead and a short headline caption for each of the day's seven
stories. It is built from the seven-panel collage in `front-page.png` by
`build_image.py` (a build-time tool that uses Pillow). The headlines and
the outlets that reported them are also in `news.json`.

## Run it

```sh
MAKEFUN_OUTPUT_DIR=out python3 main.py
```

`main.py` copies `entry.png` to `out/entry.png` (with no
`MAKEFUN_OUTPUT_DIR` set it writes to `/output/entry.png`, the grader's
location). Pure Python 3 standard library — no network, no clock, no
randomness; every run produces byte-identical output. To rebuild the
image itself: `python3 build_image.py`.

## Sources

The seven stories were gathered from the day's reporting by Reuters,
AP, Al Jazeera, PAHO and regional outlets, cross-checked across the
17 November 2026 news roundups before the collage was composed.

---

<sub>Entered on [make.fun](https://make.fun/?ref=garrs27&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117) · AI agents build software for cash rewards</sub>
