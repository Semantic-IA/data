## Simulation results

This folder contains the results of our simulations using the Simulator [TODO Link].

The top-level folders mark the different modes:

```
m1     - Completely indistinguishable blocks - randomly chosen dummies
m2     - 1 block distinguishable (1BD)       - randomly chosen dummies
m2-alt - Optimized 1BD                       - randomly chosen dummies
m3     - All blocks distinguishable (ABD)    - randomly chosen dummies
m4     - Completely indistinguishable blocks - pattern-based choice of dummies
m5     - 1 block distinguishable (1BD)       - pattern-based choice of dummies
m6     - All blocks distinguishable (ABD)    - pattern-based choice of dummies
```

Inside these folders, there are more folders, marking the used block size

```
N2   - Blocksize of 2
N5   - Blocksize of 5
N10  - Blocksize of 10
N20  - Blocksize of 20
N50  - Blocksize of 50
N100 - Blocksize of 100
N200 - Blocksize of 200
N500 - Blocksize of 500
```

Inside those folders, there are yet more folders, marking the used size of the client dataset

```
S100    - 100 queries in client dataset
S200    - 200 queries in client dataset
S500    - 500 queries in client dataset
S1000   - 1000 queries in client dataset
S2000   - 2000 queries in client dataset
S5000   - 5000 queries in client dataset
S10000  - 10,000 queries in client dataset
S20000  - 20,000 queries in client dataset
S50000  - 50,000 queries in client dataset
S100000 - 100,000 queries in client dataset
S200000 - 200,000 queries in client dataset
S-1     - all 216,925 queries in client dataset
```

Inside these folders, there are files.

```
M-{Number}.txt     - Contains k-identifiabilities for all patterns of length {number}
M-ALL.txt          - Contains k-identifiabilities for all patterns of any length
M-ALL-notNull.txt  - Identical to M-ALL.txt
M-ALL-relative.txt - Contains cumulative relative k-identifiabilities (ratios)
M-ALL-uniq.txt     - Same as -relative, but only containing lines where the ratio changed
M-ALL.txt.cont0    - Identical to M-ALL.txt, but contains k-identifiabilities with zero patterns
```

These textfiles contain their data in a `gnuplot`-compatible format.
