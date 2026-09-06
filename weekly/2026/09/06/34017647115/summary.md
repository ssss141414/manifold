### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000844`
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
| 667 | Intersect12 Q->P | 1118.60 | 0.997 | 445.00 | 670.40 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 487.20 | 0.990 | 341.40 | 140.80 | 5.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 412.20 | 0.998 | 163.00 | 248.20 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 361.20 | 0.991 | 212.00 | 146.00 | 2.20 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 163.80 | 0.972 | 72.40 | 86.80 | 1.60 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 128.80 | 0.977 | 80.60 | 45.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 102.40 | 0.961 | 57.20 | 41.20 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.40 | 1.000 | 24.00 | 18.40 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.78 | 0.92 | 0.74 | 3.83 | 4.79 | 4.66 | 4.91 | 5 |
| 2048 | 2.68 | 2.13 | 1.85 | 4.74 | 6.29 | 6.00 | 6.73 | 5 |
| 8192 | 6.78 | 5.53 | 4.93 | 10.53 | 11.68 | 11.33 | 12.86 | 5 |
| 32768 | 17.16 | 17.00 | 11.90 | 25.26 | 33.22 | 29.73 | 35.98 | 5 |
| 131072 | 58.25 | 54.04 | 42.27 | 94.29 | 121.87 | 115.52 | 130.45 | 5 |
| 524288 | 337.90 | 274.67 | 209.62 | 688.00 | 523.83 | 516.62 | 532.00 | 5 |
| 2097152 | 1385.65 | 827.30 | 783.34 | 3220.45 | 1967.35 | 1521.44 | 2090.27 | 5 |
| 8388608 | 12673.46 | 11641.10 | 10362.50 | 17385.70 | 3919.68 | 3256.14 | 4132.92 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1738.00 | 1741.00 | 1519.00 | 1962.00 | 5 |
| Boolean.BatchBoolean | 1.20 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 846.40 | 846.00 | 841.00 | 852.00 | 5 |

