### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000847`
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
| 667 | Intersect12 Q->P | 1214.40 | 0.997 | 493.80 | 717.40 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 511.00 | 0.991 | 357.20 | 149.20 | 4.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 439.60 | 0.998 | 173.00 | 265.60 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 382.80 | 0.990 | 215.20 | 163.80 | 2.80 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 168.20 | 0.973 | 74.00 | 89.60 | 1.40 | 3.20 | 5 |
| 406 | Intersect12 P->Q | 130.20 | 0.975 | 80.60 | 46.40 | 3.20 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 107.60 | 0.961 | 58.00 | 45.40 | 4.20 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 43.80 | 1.000 | 24.80 | 19.00 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.36 | 1.07 | 0.77 | 2.76 | 4.79 | 4.67 | 4.91 | 5 |
| 2048 | 2.08 | 2.09 | 1.83 | 2.33 | 6.32 | 6.23 | 6.62 | 5 |
| 8192 | 5.88 | 5.73 | 4.90 | 6.64 | 11.42 | 11.33 | 11.52 | 5 |
| 32768 | 16.24 | 16.76 | 11.66 | 18.88 | 31.87 | 29.80 | 35.48 | 5 |
| 131072 | 58.67 | 50.63 | 43.32 | 76.96 | 121.68 | 107.89 | 132.23 | 5 |
| 524288 | 248.35 | 208.28 | 199.86 | 418.07 | 530.09 | 513.58 | 543.72 | 5 |
| 2097152 | 1063.74 | 745.05 | 646.98 | 1599.85 | 1944.34 | 1414.28 | 2080.59 | 5 |
| 8388608 | 12059.58 | 10606.90 | 10168.50 | 18047.90 | 3813.21 | 3035.91 | 4249.98 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1702.00 | 1717.00 | 1504.00 | 1866.00 | 5 |
| Boolean.BatchBoolean | 2.40 | 2.00 | 1.00 | 4.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.40 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 886.40 | 815.00 | 800.00 | 1089.00 | 5 |

