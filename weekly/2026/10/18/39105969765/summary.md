### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000862`
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
| 667 | Intersect12 Q->P | 1409.80 | 0.997 | 533.60 | 872.40 | 0.00 | 3.80 | 5 |
| 695 | Intersect12 P->Q | 667.40 | 0.992 | 445.40 | 216.80 | 5.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 503.60 | 0.998 | 206.80 | 295.80 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 433.20 | 0.990 | 260.00 | 169.20 | 3.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 216.40 | 0.971 | 94.00 | 116.20 | 2.00 | 4.20 | 5 |
| 406 | Intersect12 P->Q | 168.20 | 0.974 | 106.00 | 57.80 | 4.40 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 162.20 | 0.965 | 87.20 | 69.60 | 5.40 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 50.00 | 0.997 | 28.00 | 21.80 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 3.07 | 2.82 | 1.13 | 4.94 | 4.72 | 4.50 | 4.78 | 5 |
| 2048 | 3.64 | 3.79 | 2.26 | 4.69 | 6.33 | 5.83 | 6.55 | 5 |
| 8192 | 13.48 | 14.24 | 7.83 | 18.21 | 12.29 | 11.19 | 13.22 | 5 |
| 32768 | 31.46 | 32.16 | 23.57 | 39.52 | 34.13 | 32.53 | 36.06 | 5 |
| 131072 | 147.00 | 137.70 | 81.11 | 233.47 | 122.28 | 113.16 | 134.75 | 5 |
| 524288 | 725.28 | 642.72 | 456.44 | 1130.89 | 524.58 | 500.64 | 538.02 | 5 |
| 2097152 | 2331.76 | 2336.60 | 1443.27 | 3712.55 | 1965.91 | 1462.84 | 2095.09 | 5 |
| 8388608 | 23104.30 | 21904.70 | 16692.30 | 30930.80 | 3685.52 | 2882.98 | 3943.03 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2313.20 | 2224.00 | 1869.00 | 2778.00 | 5 |
| Boolean.BatchBoolean | 2.40 | 2.00 | 2.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 1.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.80 | 3.00 | 2.00 | 4.00 | 5 |
| Polygon.Zebra3 | 1243.80 | 1252.00 | 1073.00 | 1411.00 | 5 |

