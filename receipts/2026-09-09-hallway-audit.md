# Receipt — hallway mechanical audit

- When: 2026-09-09
- Who: HERMOSA pass via connected git `rgiskard01-fiddler` (cannot write `DavidWise01/0root`; 403)
- What was counted: every `<a class="sph">` href on https://davidwise01.github.io/ud0/the-index.html
- Method: concurrent HEAD, GET fallback on 403/405/501, 32 workers, 12s timeout
- Result: **4176 / 4176 HTTP 200**. Failures: 0.

World split of those hrefs:

```
W1 CORPUS   2049
W2 FOLD     2048
W4 SONIA      48
W5 SONNY 5    31
--------------
spheres     4176
W3 stewards    8   (.sph chips, not <a class="sph">)
items       4184
```

Sample of 40 pages across I/II/IV/V: all 200. LIT/AMBER/WALL words appear on many pages; a string count is not a self-check. Two corpus pages in the sample (`the-heap`, `willard-van-orman-quine`) contain both `throw` and `self-check`. Fold/Sonia/Sonny pages often carry LIT+AMBER+WALL labels. That is AMBER evidence of labeling, not LIT proof every computation ran.

## Fixes applied on this fork only

`DavidWise01/0root` rejected writes (GitHub 403). Patches live on `rgiskard01-fiddler/0root`:

1. `index.html` — SONIA footer 1 → 48; SONIA stat 1 sphere / 4 rooms → 48 spheres / 5 rooms; SONNY 5 stat drops the unverified "25 darts, climbing to 2048" clause (31 catalog spheres remain).
2. `README.md` — five worlds, not three; dated catalog table.
3. `llms.txt` — dated AMBER snapshot; INDEX remains source of truth.

No `.dlw` seal was rewritten.

## Not fixed (needs ROOT0 / `DavidWise01` auth)

- Merge this fork onto `DavidWise01/0root` so `0root.ai` updates.
- Make the hallway footer a live read of THE INDEX instead of a frozen sentence.
- Exhaustive LIT execution of 2,048 fold pages.
- W2 domain badge 64 vs 65 `.dom` nodes on THE INDEX.
