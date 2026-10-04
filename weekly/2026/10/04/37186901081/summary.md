### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000856`
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
| 667 | Intersect12 Q->P | 1233.80 | 0.998 | 503.80 | 727.00 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 539.60 | 0.990 | 365.80 | 168.20 | 5.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 425.40 | 0.997 | 166.20 | 257.80 | 0.00 | 1.40 | 5 |
| 84 | Intersect12 P->Q | 419.60 | 0.991 | 250.20 | 165.60 | 2.80 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 193.20 | 0.971 | 85.40 | 102.40 | 2.00 | 3.40 | 5 |
| 406 | Intersect12 P->Q | 136.60 | 0.975 | 83.00 | 50.20 | 3.40 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 120.80 | 0.957 | 64.60 | 51.00 | 5.20 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.20 | 1.000 | 24.00 | 18.20 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 2.82 | 1.56 | 0.80 | 8.69 | 4.71 | 4.48 | 4.92 | 5 |
| 2048 | 3.70 | 3.14 | 1.92 | 6.69 | 6.09 | 5.69 | 6.39 | 5 |
| 8192 | 12.65 | 8.36 | 5.05 | 33.16 | 11.96 | 11.31 | 13.19 | 5 |
| 32768 | 21.10 | 21.74 | 12.17 | 32.78 | 34.76 | 30.94 | 37.56 | 5 |
| 131072 | 123.55 | 122.47 | 43.70 | 188.13 | 124.94 | 115.27 | 134.41 | 5 |
| 524288 | 596.45 | 604.54 | 341.29 | 822.52 | 533.52 | 525.39 | 540.94 | 5 |
| 2097152 | 1752.91 | 1773.74 | 1029.92 | 2234.80 | 2006.03 | 1710.28 | 2089.19 | 5 |
| 8388608 | 19667.58 | 21737.20 | 11859.50 | 23417.30 | 3665.17 | 3068.78 | 3966.19 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2393.60 | 2203.00 | 1908.00 | 3359.00 | 5 |
| Boolean.BatchBoolean | 2.80 | 2.00 | 2.00 | 4.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 1.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1286.40 | 1343.00 | 1059.00 | 1480.00 | 5 |

