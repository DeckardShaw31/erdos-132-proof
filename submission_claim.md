# Official Submission Package: Erdős Problem #132

This document contains everything needed to submit your findings to **erdosproblems.com** and open a Pull Request to the GitHub repository **teorth/erdosproblems**.

---

## Part 1: Submission Form on `erdosproblems.com`

**Submit URL**: [https://www.erdosproblems.com/forum/thread/132/submit-proof](https://www.erdosproblems.com/forum/thread/132/submit-proof)

Copy and paste the following into the website form fields:

### Field 1: Author(s)
```text
Nguyễn Nhật Thanh
```

### Field 2: AI models used (if any)
```text
Gemini 2.5 Pro / Antigravity AI assistant
```

### Field 3: Please tick if this is a partial proof
```text
[X] TICK THIS BOX (Checked / Yes)
```
*(Explanation: The paper affirmatively settles n = 7 and n = 8, but the general conjecture for all n remains open).*

### Field 4: URL to a human-readable writeup of the proof (use an arXiv link if available)
```text
https://github.com/DeckardShaw31/erdos-132-proof/blob/main/main.pdf
```
*(Note: If you name your repository differently, replace `erdos-132-proof` with your repository name. You can also link `https://github.com/DeckardShaw31/erdos-132-proof` or an OSF / Zenodo / arXiv link).*

### Field 5: URL to a Lean formalisation of the proof, if available
*(Leave blank / N/A)*

### Field 6: A short summary of what is claimed, and the main ideas of the proof
```text
We prove Erdős Problem #132 affirmatively for n = 7 and n = 8.

By the Hopf–Pannwitz diameter bound and pair counting, any counterexample cannot have rare distances other than the diameter, restricting possible distance multiplicities to 9 candidate integer partitions for n = 7 and 11 for n = 8. We show through geometric variance minimization that none of these partitions admits an isometric embedding in the Euclidean plane, establishing that every 7- and 8-point planar set determines at least two rare distances.
```

### Field 7: Any additional notes
```text
This work establishes n = 7 and provides an independent, classification-free computational certification for n = 8 (complementing Beller's Lean formalisation). Standalone reproduction scripts (verify_n7.py and verify_n8.py) with zero external dependencies beyond NumPy and SciPy are included in the repository. The general problem for all n remains open.
```

---

## Part 2: Step-by-Step GitHub Setup for Your Paper URL

To generate your live public link before hitting submit on the website:

1. Open your browser and go to [https://github.com/new](https://github.com/new).
2. Name the repository: `erdos-132-proof` (set to **Public**). Do NOT add a README or .gitignore (we already have them).
3. In PowerShell in `c:\Users\proin\Desktop\bountyhunt\132`, run:
   ```powershell
   git remote add origin https://github.com/DeckardShaw31/erdos-132-proof.git
   git branch -M main
   git push -u origin main
   ```
4. Once pushed, `main.pdf`, `paper.tex`, `verify_n7.py`, and `verify_n8.py` will be live and publicly viewable at:
   `https://github.com/DeckardShaw31/erdos-132-proof`

---

## Part 3: GitHub PR for `teorth/erdosproblems`

To update the main tracking database at [https://github.com/teorth/erdosproblems](https://github.com/teorth/erdosproblems):

1. **Fork** `teorth/erdosproblems` on GitHub.
2. In `data/problems.yaml`, locate entry `number: "132"` (around line 2158) and update `informal_status`:
   ```yaml
   - number: "132"
     prize: "$100"
     informal_status:
       state: "open"
       last_update: "2026-09-10"
       note: "Proved for convex sets (CDL 2025); verified for n in {5,6,7,8} (Erdos-Fishburn 1996, Thanh 2026)."
     formal_status:
       state: "unformalized"
     status:
       state: "open"
       last_update: "2026-09-10"
     oeis: ["N/A"]
     formalized:
       state: "no"
       last_update: "2025-08-31"
     tags: ["distances"]
   ```
3. Open a Pull Request titled:  
   `Update note for Problem #132: note verification for n=7 and n=8`
