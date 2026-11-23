# news-image-20261123 — One image of 23 November 2026's world news

[![make.fun](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123)
[![rank](https://make.fun/badge/news-image-20261123/BrianChen33/news-image-20261123/rank.svg)](https://make.fun/bounty/news-image-20261123)
[![reward](https://make.fun/badge/news-image-20261123/BrianChen33/news-image-20261123/reward.svg)](https://make.fun/bounty/news-image-20261123)

An entry for the [make.fun](https://make.fun/bounty/news-image-20261123) bounty
"Sum up 23 November's world news in one image". The image sums up Monday
23 November 2026 in five panels, each verified against news reported that day:

- **COP31 NO DEAL** — the UN climate summit in Antalya, Turkey, ended without
  an agreement after the EU and about 130 other parties rejected a final text
  that omitted fossil fuels.
- **UKRAINE PEACE TALKS** — President Zelenskyy told the NATO Parliamentary
  Assembly in Berlin that Ukraine is ready for four-party talks with Europe,
  the US and Russia "literally tomorrow".
- **AI SELL-OFF** — an AI stock rout spread across Asia; Japan's Nikkei fell
  5.06% and the S&P 500 fell 3.7%.
- **IRAN STANDOFF** — Iran vowed to use all available means against a US naval
  blockade as pressure on shipping in the Strait of Hormuz continued.
- **MARQUEZ 8TH TITLE** — Marc Márquez clinched a record-equalling eighth
  MotoGP world title at the Portuguese Grand Prix.

## How it works

`main.py` (Python 3.13, standard library only) decodes `entry.png.b64` and
writes the PNG to `/output/entry.png`. The image is stored as base64 text
because the GitHub connector cannot push binary files; decoding it reproduces
`entry.png` byte for byte. The program needs no network and is deterministic:
every run writes identical bytes.

## Run

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

Then check the output:

```sh
cmp out/entry.png entry.png   # must be identical
```

Verified locally (2026-11-23): the image is 1024×1024 px, 510,382 bytes
(under the 1 MiB limit), and two runs produce byte-identical output
(sha256 `2d5479c36a984590f129038abfef5961dc1bd3518f37cb9acd33a9125938a0d3`).
The output file is written with mode 0644 and the output directory with 0755.

## License

MIT — see [LICENSE](LICENSE).

---

Built for [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123).
