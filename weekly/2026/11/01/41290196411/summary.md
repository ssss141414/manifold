### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000868`
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
| 667 | Intersect12 Q->P | 1136.60 | 0.997 | 452.60 | 681.00 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 485.60 | 0.991 | 337.00 | 144.40 | 4.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 417.00 | 0.998 | 166.00 | 250.00 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 390.00 | 0.991 | 225.40 | 161.20 | 2.40 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 167.20 | 0.971 | 75.60 | 86.80 | 1.80 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 132.40 | 0.977 | 82.80 | 46.60 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 101.80 | 0.961 | 57.00 | 40.80 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 43.80 | 1.000 | 25.20 | 18.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.64 | 1.45 | 0.94 | 2.42 | 4.62 | 4.36 | 4.78 | 5 |
| 2048 | 4.67 | 4.67 | 2.31 | 9.30 | 6.38 | 5.98 | 6.73 | 5 |
| 8192 | 10.00 | 7.13 | 5.59 | 17.84 | 12.38 | 11.48 | 13.52 | 5 |
| 32768 | 19.96 | 19.89 | 12.72 | 30.70 | 33.35 | 29.70 | 37.16 | 5 |
| 131072 | 217.14 | 264.99 | 44.67 | 373.56 | 127.52 | 117.92 | 137.91 | 5 |
| 524288 | 527.46 | 457.48 | 425.81 | 685.54 | 526.89 | 521.50 | 532.08 | 5 |
| 2097152 | 1611.34 | 1417.14 | 1322.14 | 2304.43 | 2025.65 | 1797.94 | 2092.75 | 5 |
| 8388608 | 18582.00 | 18765.50 | 13635.70 | 23194.50 | 3800.14 | 3362.58 | 4009.17 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 3738.00 | 3295.00 | 3178.00 | 5309.00 | 5 |
| Boolean.BatchBoolean | 4.00 | 3.00 | 2.00 | 7.00 | 5 |
| CrossSection.BatchBoolean | 0.60 | 0.00 | 0.00 | 3.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 0.00 | 2.00 | 5 |
| Polygon.Zebra1 | 3.60 | 4.00 | 2.00 | 5.00 | 5 |
| Polygon.Zebra3 | 1577.20 | 1562.00 | 1305.00 | 1864.00 | 5 |

