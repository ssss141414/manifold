### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000859`
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
| 667 | Intersect12 Q->P | 1198.00 | 0.997 | 486.00 | 708.80 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 503.40 | 0.988 | 343.20 | 154.20 | 6.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 439.40 | 0.997 | 175.40 | 262.80 | 0.00 | 1.20 | 5 |
| 84 | Intersect12 P->Q | 395.40 | 0.991 | 227.80 | 164.00 | 2.60 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 184.00 | 0.972 | 87.20 | 91.60 | 2.00 | 3.20 | 5 |
| 406 | Intersect12 P->Q | 130.20 | 0.971 | 80.60 | 45.80 | 3.80 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 120.20 | 0.960 | 66.40 | 49.00 | 4.80 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 48.00 | 0.997 | 27.80 | 20.00 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 3.39 | 1.48 | 0.76 | 11.63 | 4.70 | 4.47 | 4.95 | 5 |
| 2048 | 2.42 | 2.34 | 1.87 | 3.32 | 6.16 | 5.64 | 6.72 | 5 |
| 8192 | 8.31 | 6.76 | 5.12 | 15.91 | 11.90 | 11.20 | 13.53 | 5 |
| 32768 | 22.19 | 19.76 | 12.48 | 33.91 | 35.19 | 30.55 | 37.23 | 5 |
| 131072 | 123.53 | 133.88 | 61.50 | 160.05 | 125.06 | 111.09 | 134.83 | 5 |
| 524288 | 553.17 | 556.55 | 428.31 | 676.27 | 532.30 | 522.95 | 547.53 | 5 |
| 2097152 | 1450.31 | 1403.10 | 1214.67 | 1835.30 | 2026.10 | 1789.17 | 2095.11 | 5 |
| 8388608 | 18647.34 | 17924.80 | 15093.50 | 22709.10 | 3676.34 | 3076.34 | 3889.94 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 3181.20 | 3244.00 | 2753.00 | 3380.00 | 5 |
| Boolean.BatchBoolean | 3.80 | 4.00 | 2.00 | 6.00 | 5 |
| CrossSection.BatchBoolean | 0.40 | 0.00 | 0.00 | 2.00 | 5 |
| Polygon.Sponge4 | 1.40 | 1.00 | 1.00 | 2.00 | 5 |
| Polygon.Zebra1 | 3.80 | 3.00 | 2.00 | 6.00 | 5 |
| Polygon.Zebra3 | 1599.40 | 1650.00 | 1415.00 | 1713.00 | 5 |

