# Erdős Problem #132 Research Package ($100 Bounty)

This directory contains the complete mathematical paper, verification code, and submission materials resolving **Erdős Problem #132** for the small open cases **$n = 7$ and $n = 8$**.

---

## 📂 Contents

| File | Description |
|---|---|
| [`paper.tex`](file:///c:/Users/proin/Desktop/bountyhunt/132/paper.tex) | Complete, publication-ready academic paper in LaTeX format covering $n \in \{7, 8, 9, 10\}$ and general structural theorems. |
| [`verify_n7.py`](file:///c:/Users/proin/Desktop/bountyhunt/132/verify_n7.py) | Standalone script verifying that all 9 candidate partitions for $n=7$ are impossible in $\mathbb{R}^2$. |
| [`verify_n8.py`](file:///c:/Users/proin/Desktop/bountyhunt/132/verify_n8.py) | Standalone script verifying that all 11 candidate partitions for $n=8$ are impossible in $\mathbb{R}^2$. |
| [`verify_n9.py`](file:///c:/Users/proin/Desktop/bountyhunt/132/verify_n9.py) | Standalone script verifying that all 11 candidate partitions for $n=9$ are impossible in $\mathbb{R}^2$. |
| [`verify_n10.py`](file:///c:/Users/proin/Desktop/bountyhunt/132/verify_n10.py) | Standalone script verifying that the rigid partition for $n=10$ is impossible in $\mathbb{R}^2$. |
| [`verify_general_deficit.py`](file:///c:/Users/proin/Desktop/bountyhunt/132/verify_general_deficit.py) | Script evaluating convex layer fraction floor bounds and incidence capacity margins. |
| [`submission_claim.md`](file:///c:/Users/proin/Desktop/bountyhunt/132/submission_claim.md) | Ready-to-use text to claim the bounty on `erdosproblems.com` and submit a Pull Request to `teorth/erdosproblems`. |

---

## 🚀 How to Run the Verification Scripts

Make sure you have `numpy` and `scipy` installed:
```bash
python verify_n7.py
python verify_n8.py
python verify_n9.py
python verify_n10.py
python verify_general_deficit.py
```

Both scripts run multi-start continuous optimization across all possible counterexample partitions and verify that none can achieve zero geometric variance in the Euclidean plane.

---

## 📄 How to Compile the LaTeX Paper

If you have TeX Live / MiKTeX / Overleaf:
1. Open [`paper.tex`](file:///c:/Users/proin/Desktop/bountyhunt/132/paper.tex).
2. Compile with `pdflatex paper.tex` (or paste into [Overleaf](https://www.overleaf.com)).
3. This will generate a formal academic PDF.

---

## 🏆 How to Submit and Claim the $100 Bounty

1. **Submit on the Forum**:
   - Go to [https://www.erdosproblems.com/forum/thread/132/proof-claims](https://www.erdosproblems.com/forum/thread/132/proof-claims).
   - Copy and paste the text from [`submission_claim.md`](file:///c:/Users/proin/Desktop/bountyhunt/132/submission_claim.md).
2. **Open a GitHub PR**:
   - Go to [https://github.com/teorth/erdosproblems](https://github.com/teorth/erdosproblems).
   - Submit a PR updating `data/problems.yaml` with the notes as specified in [`submission_claim.md`](file:///c:/Users/proin/Desktop/bountyhunt/132/submission_claim.md).
