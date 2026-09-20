### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000850`
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
| 667 | Intersect12 Q->P | 1589.60 | 0.997 | 625.40 | 960.00 | 0.00 | 4.20 | 5 |
| 695 | Intersect12 P->Q | 645.80 | 0.989 | 447.60 | 191.20 | 6.80 | 0.20 | 5 |
| 16 | Intersect12 Q->P | 528.00 | 0.996 | 209.00 | 317.00 | 0.00 | 2.00 | 5 |
| 84 | Intersect12 P->Q | 479.40 | 0.992 | 270.20 | 205.20 | 3.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 236.80 | 0.975 | 106.60 | 124.20 | 2.00 | 4.00 | 5 |
| 406 | Intersect12 P->Q | 166.40 | 0.977 | 103.40 | 59.20 | 3.80 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 140.00 | 0.964 | 76.00 | 59.00 | 5.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 56.00 | 0.997 | 32.80 | 23.00 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.88 | 1.51 | 1.36 | 3.10 | 4.66 | 4.47 | 4.97 | 5 |
| 2048 | 4.31 | 3.91 | 3.12 | 6.15 | 6.15 | 5.86 | 6.66 | 5 |
| 8192 | 13.37 | 9.24 | 6.82 | 29.15 | 12.86 | 10.86 | 14.16 | 5 |
| 32768 | 28.64 | 19.36 | 17.06 | 54.86 | 34.53 | 32.31 | 36.41 | 5 |
| 131072 | 116.62 | 102.68 | 63.68 | 223.41 | 123.58 | 116.86 | 129.14 | 5 |
| 524288 | 667.02 | 663.42 | 354.44 | 1221.04 | 526.52 | 494.02 | 540.31 | 5 |
| 2097152 | 1935.27 | 2007.09 | 1254.41 | 2429.12 | 1970.55 | 1510.56 | 2090.45 | 5 |
| 8388608 | 21408.16 | 22647.80 | 16831.50 | 24191.30 | 3714.83 | 2958.53 | 4004.75 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2796.40 | 2601.00 | 2551.00 | 3465.00 | 5 |
| Boolean.BatchBoolean | 3.00 | 2.00 | 2.00 | 6.00 | 5 |
| CrossSection.BatchBoolean | 0.40 | 0.00 | 0.00 | 2.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 1.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1334.40 | 1248.00 | 1230.00 | 1671.00 | 5 |

