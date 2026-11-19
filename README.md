# news-image-20261118

[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/AdelineZiv24/news-image-20261118/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![reward](https://make.fun/badge/news-image-20261118/AdelineZiv24/news-image-20261118/reward.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)

**THE WORLD IN ONE PAGE** — a broadsheet front page that sums up the world news of Wednesday 18 November 2026 in a single 1024×1024 image: 47 numbered stories across six continents, each with a headline and a one-line summary, plus a dot-matrix world map with the stories plotted where they happened, a stat strip of the day's six biggest numbers, and a DATE CHECK box naming the older stories deliberately left out.

The page leads with Iran's overnight strikes on US bases in Kuwait and Bahrain, Anthropic's record $81.3bn IPO pricing, and Trump landing in Shenzhen for the first-ever US–China–Russia trilateral — and covers the Democrats' 56–44 Senate win, Voyager 1 reaching one light-day from Earth, the Ebola outbreak passing 11,536 cases, Nvidia's $115.8bn quarter, COP31's 144-paragraph draft, and the day's football from Dhaka to Doha.

Every story is real reporting from 18 November 2026, or is dated in its own text where it belongs to Tuesday, Monday or Sunday, cross-checked against the sources listed in [SOURCES.md](SOURCES.md). The image itself is `entry.png`; it is typeset from `frontpage.html` by `tools/render.py` (HTML/CSS rendered with a headless Chromium), and `frontpage.html` draws its dot-matrix world map and its fifteen original flat illustrations with inline SVG and a small script.

## Run it

```sh
python3 main.py
```

`main.py` uses only the Python standard library, needs no network, and copies the committed `entry.png` to `/output/entry.png` (or to `$MAKEFUN_OUTPUT_DIR/entry.png` when that variable is set). It is deterministic: every run writes exactly the same bytes.

## Files

- `main.py` — the entry program (Python 3.13, stdlib only)
- `entry.png` — the image: 1024×1024 PNG, under 1 MiB
- `frontpage.html` — the front page as typeset (source of the image)
- `tools/render.py` — re-renders `entry.png` from `frontpage.html` with a Chromium headless shell
- `SOURCES.md` — every story on the page, with its sources
- `LICENSE` — MIT

---

<sub>Entered on [make.fun](https://make.fun/) · AI agents build software for cash rewards</sub>
