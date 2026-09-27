### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000853`
OS: `macOS`
Compiler: `AppleClang 17.0.0.17000013`
CPU: `Apple M1 (Virtual)`
CPU count: `3`
CPU model identifier: `VirtualMac2,1`
CPU physical cores: `3`
CPU performance cores: `3`
Repeats: `5`

#### Ember Phase Timings

| Case | Dominant phase | Full mean (ms) | Intersect12 share | P->Q | Q->P | Winding P | Winding Q | Runs |
|---:|---|---:|---:|---:|---:|---:|---:|---:|
| 667 | Intersect12 Q->P | 1311.80 | 0.997 | 517.80 | 790.00 | 0.00 | 4.00 | 5 |
| 695 | Intersect12 P->Q | 515.20 | 0.990 | 358.40 | 151.60 | 5.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 457.20 | 0.997 | 177.20 | 278.80 | 0.00 | 1.20 | 5 |
| 84 | Intersect12 P->Q | 428.20 | 0.988 | 243.00 | 180.20 | 3.40 | 1.60 | 5 |
| 260 | Intersect12 Q->P | 181.80 | 0.967 | 78.80 | 97.00 | 2.00 | 4.00 | 5 |
| 406 | Intersect12 P->Q | 141.00 | 0.976 | 87.40 | 50.20 | 3.40 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 112.00 | 0.959 | 62.60 | 44.80 | 4.60 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 47.20 | 1.000 | 26.80 | 20.40 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.12 | 1.05 | 0.91 | 1.62 | 4.77 | 4.75 | 4.80 | 5 |
| 2048 | 2.83 | 2.60 | 2.19 | 4.19 | 6.54 | 6.23 | 6.73 | 5 |
| 8192 | 6.92 | 6.60 | 6.23 | 7.79 | 11.63 | 11.33 | 11.95 | 5 |
| 32768 | 21.74 | 17.67 | 15.28 | 35.98 | 35.42 | 29.80 | 39.75 | 5 |
| 131072 | 61.77 | 54.81 | 54.19 | 79.42 | 125.16 | 120.48 | 130.48 | 5 |
| 524288 | 427.77 | 341.25 | 272.42 | 862.55 | 524.19 | 518.89 | 529.38 | 5 |
| 2097152 | 1667.67 | 1147.04 | 881.17 | 3673.95 | 1954.31 | 1453.81 | 2083.62 | 5 |
| 8388608 | 15126.78 | 11956.00 | 11019.60 | 26070.20 | 3919.39 | 2919.70 | 4237.31 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1955.20 | 1933.00 | 1722.00 | 2126.00 | 5 |
| Boolean.BatchBoolean | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 1.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1051.00 | 1027.00 | 998.00 | 1165.00 | 5 |

