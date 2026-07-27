# Sigma Katapayadi — GoPada Padhathi

A single-file, offline browser tool that maps names to zodiac coordinates using a **summation reformulation** of the classical Katapayadi system. Part of the **Nama Kanda** research framework by Astrogaami.

**Live tool:** `https://<your-username>.github.io/sigma-katapayadi/`
*(replace `<your-username>` after you enable GitHub Pages, see below)*

---

## What it is

Classical Katapayadi turns consonants into digits so a number can be hidden inside a word. It **concatenates** those digits into one place-value number, read right to left (*aṅkānāṃ vāmato gatiḥ*).

Sigma Katapayadi keeps the same consonant-to-digit grid but changes one step: instead of concatenating, it **sums** the digits into a single value, Sigma (Σ). That one change turns an encoding cipher into a mapping instrument, because Σ can then be projected onto the wheels of a chart:

- **Σ mod 12 → Nama Rashi** (the Name Sign)
- **Σ mod 7 → seven-graha lord**
- **Σ mod 9 → nine-graha lord**
- **Σ mod 27 → Nama Nakshatra**

A second layer reads the **first sounding consonant** as a Varna Graha (planetary lord of the opening syllable), following the Agni Purana varga grouping.

Because summation is order-independent, the result is invariant to reading direction, so the old reversal ambiguity simply does not arise.

## The four rules (extraction)

1. **Only consonants carry value.** Vowels, matras, anusvara and visarga are silent.
2. **In a conjunct, only the last consonant sounds.** Dead (halant-bound) consonants are dropped.
3. **A standalone vowel is zero.**
4. **Sum the digits** to get Σ, then take the moduli above.

## Features

- Enter names in Devanagari (e.g. `राम, कृष्ण, ज्योति`) or plain numbers (e.g. `108`)
- Add multiple names at once and compute in a batch
- **Review Syllables** to see the per-akshara digit breakdown
- Reference panels: Katapayadi map, First-Letter (Varna Graha) mapping, the rules, Rashi table, planet tables, and the 27 nakshatras
- **Export CSV** and **Copy for book** for manuscript work
- Runs fully offline, no server, no tracking, no external libraries

## How to use

Open the live link above, or download `index.html` and open it in any modern browser. That is all, there is no install step.

## Status and epistemic note

Sigma Katapayadi is an **original, exploratory research framework**, offered as a contribution to the Jyotisha community. The name-to-sign mapping is a proposed technique under active empirical testing; it is **not** an established or independently validated result. Illustrative chart examples show the method fitting known cases, which is a starting point for investigation, not proof. A proper test requires pre-registered connection rules, a measured base rate against random charts, and a convergence study on independent name-pairs. Readers are encouraged to test it critically rather than accept it on the strength of selected examples.

## Repository layout

```
sigma-katapayadi/
├── index.html         # the tool (GitHub Pages serves this)
├── SigmaKatapayadi_Numerology_Lite_v9e.html   # original versioned filename (identical copy)
├── README.md
├── LICENSE
├── CITATION.cff
└── .gitignore
```

## Citing

If you reference this method or tool, please cite it (see `CITATION.cff`) and credit **Astrogaami**.

## License

Released under **CC BY-NC-SA 4.0**: free to use, share and adapt for non-commercial purposes, with attribution, under the same license. See `LICENSE`.

## Acknowledgements

Developed by Astrogaami as part of the Nama Kanda work. Offered as a gift to the Jyotisha community.
