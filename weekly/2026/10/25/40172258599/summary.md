### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000865`
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
| 667 | Intersect12 Q->P | 1364.40 | 0.997 | 518.60 | 841.60 | 0.00 | 4.20 | 5 |
| 695 | Intersect12 P->Q | 559.20 | 0.990 | 384.60 | 169.20 | 5.40 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 530.60 | 0.998 | 205.00 | 324.60 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 524.20 | 0.990 | 309.00 | 210.00 | 3.80 | 1.40 | 5 |
| 260 | Intersect12 Q->P | 226.00 | 0.969 | 102.20 | 116.80 | 2.80 | 4.20 | 5 |
| 406 | Intersect12 P->Q | 151.00 | 0.979 | 92.20 | 55.60 | 3.20 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 120.80 | 0.958 | 65.60 | 50.00 | 5.00 | 0.20 | 5 |
| 582 | Intersect12 P->Q | 47.20 | 1.000 | 26.60 | 20.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 2.91 | 2.65 | 0.97 | 5.49 | 4.58 | 4.36 | 4.84 | 5 |
| 2048 | 3.73 | 4.32 | 1.99 | 4.83 | 6.35 | 6.03 | 6.64 | 5 |
| 8192 | 11.92 | 10.21 | 5.18 | 20.04 | 12.34 | 11.31 | 12.98 | 5 |
| 32768 | 30.03 | 23.41 | 13.11 | 58.48 | 35.56 | 32.28 | 37.02 | 5 |
| 131072 | 173.83 | 165.26 | 50.69 | 294.83 | 125.97 | 119.80 | 133.19 | 5 |
| 524288 | 511.08 | 496.28 | 395.71 | 735.35 | 530.12 | 526.73 | 534.36 | 5 |
| 2097152 | 1852.71 | 2013.94 | 1348.82 | 2145.98 | 1990.00 | 1628.89 | 2101.61 | 5 |
| 8388608 | 20199.14 | 20380.40 | 18773.90 | 22133.60 | 3735.54 | 3321.27 | 3936.62 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2952.40 | 2794.00 | 2522.00 | 3971.00 | 5 |
| Boolean.BatchBoolean | 5.80 | 5.00 | 2.00 | 12.00 | 5 |
| CrossSection.BatchBoolean | 0.80 | 0.00 | 0.00 | 3.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 1.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1229.00 | 1150.00 | 1087.00 | 1489.00 | 5 |

