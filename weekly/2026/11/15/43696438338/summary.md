### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000874`
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
| 667 | Intersect12 Q->P | 1128.20 | 0.997 | 449.00 | 676.20 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 533.80 | 0.991 | 376.40 | 152.60 | 4.80 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 409.20 | 0.998 | 159.20 | 249.00 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 349.40 | 0.991 | 203.40 | 143.00 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 P->Q | 186.40 | 0.976 | 91.40 | 90.60 | 1.40 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 127.60 | 0.976 | 80.00 | 44.60 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 103.20 | 0.961 | 58.00 | 41.20 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.60 | 1.000 | 24.00 | 18.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.53 | 1.05 | 0.80 | 3.74 | 4.75 | 4.45 | 4.86 | 5 |
| 2048 | 2.21 | 2.15 | 2.05 | 2.57 | 6.09 | 5.72 | 6.25 | 5 |
| 8192 | 7.80 | 6.73 | 5.62 | 12.17 | 11.97 | 10.72 | 13.33 | 5 |
| 32768 | 18.85 | 16.78 | 13.68 | 26.74 | 36.65 | 31.28 | 41.92 | 5 |
| 131072 | 123.39 | 119.89 | 48.86 | 235.28 | 131.44 | 122.08 | 141.89 | 5 |
| 524288 | 508.49 | 484.39 | 353.24 | 695.56 | 546.01 | 531.81 | 565.02 | 5 |
| 2097152 | 1514.94 | 1544.23 | 960.23 | 1904.99 | 2023.49 | 1781.28 | 2099.86 | 5 |
| 8388608 | 15934.64 | 14766.60 | 13153.20 | 19456.60 | 3665.59 | 3141.38 | 4070.80 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2777.00 | 2662.00 | 2393.00 | 3455.00 | 5 |
| Boolean.BatchBoolean | 3.00 | 2.00 | 2.00 | 5.00 | 5 |
| CrossSection.BatchBoolean | 0.40 | 0.00 | 0.00 | 2.00 | 5 |
| Polygon.Sponge4 | 0.80 | 1.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.60 | 3.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1359.40 | 1332.00 | 1139.00 | 1725.00 | 5 |

