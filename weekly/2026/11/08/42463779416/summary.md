### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000871`
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
| 667 | Intersect12 Q->P | 1477.60 | 0.997 | 590.40 | 882.60 | 0.00 | 4.60 | 5 |
| 695 | Intersect12 P->Q | 606.00 | 0.990 | 420.80 | 179.00 | 6.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 557.00 | 0.997 | 221.00 | 334.20 | 0.20 | 1.60 | 5 |
| 84 | Intersect12 P->Q | 482.40 | 0.991 | 286.40 | 191.40 | 3.40 | 1.20 | 5 |
| 260 | Intersect12 Q->P | 223.00 | 0.967 | 96.00 | 119.80 | 2.20 | 5.00 | 5 |
| 406 | Intersect12 P->Q | 161.00 | 0.978 | 99.00 | 58.40 | 3.60 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 143.00 | 0.962 | 82.00 | 55.40 | 5.60 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 71.00 | 0.992 | 38.00 | 32.40 | 0.60 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 3.35 | 1.36 | 1.10 | 10.70 | 4.73 | 4.55 | 4.84 | 5 |
| 2048 | 2.72 | 2.42 | 2.25 | 3.80 | 6.21 | 6.19 | 6.23 | 5 |
| 8192 | 9.21 | 10.46 | 5.48 | 11.29 | 12.88 | 11.33 | 13.97 | 5 |
| 32768 | 25.68 | 24.85 | 19.25 | 34.96 | 35.75 | 33.89 | 39.69 | 5 |
| 131072 | 144.12 | 184.28 | 70.45 | 191.07 | 121.79 | 114.30 | 130.53 | 5 |
| 524288 | 669.71 | 686.12 | 566.50 | 752.14 | 530.98 | 520.69 | 546.08 | 5 |
| 2097152 | 2061.54 | 2046.33 | 1401.44 | 2611.31 | 2029.72 | 1767.28 | 2102.70 | 5 |
| 8388608 | 23981.40 | 22944.40 | 20433.10 | 29840.00 | 3682.27 | 3050.12 | 4010.56 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2749.40 | 2646.00 | 2531.00 | 3145.00 | 5 |
| Boolean.BatchBoolean | 2.00 | 2.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.80 | 1.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.80 | 2.00 | 2.00 | 5.00 | 5 |
| Polygon.Zebra3 | 1234.60 | 1240.00 | 1127.00 | 1340.00 | 5 |

