### Weekly Benchmarks

Commit: `15224126a430dbfaf8ffc4a18d07935cdc5c48ec`
Runner: `GitHub Actions 1000000841`
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
| 667 | Intersect12 Q->P | 1490.20 | 0.997 | 597.40 | 888.20 | 0.00 | 4.60 | 5 |
| 695 | Intersect12 P->Q | 678.40 | 0.989 | 471.40 | 199.40 | 7.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 564.60 | 0.998 | 220.60 | 342.60 | 0.00 | 1.40 | 5 |
| 84 | Intersect12 P->Q | 479.80 | 0.991 | 274.20 | 201.00 | 3.60 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 239.60 | 0.965 | 108.80 | 122.80 | 2.80 | 5.20 | 5 |
| 406 | Intersect12 P->Q | 173.00 | 0.978 | 110.20 | 59.00 | 3.80 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 137.80 | 0.963 | 76.60 | 56.20 | 5.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 59.00 | 0.989 | 31.00 | 27.40 | 0.60 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.51 | 1.42 | 1.20 | 2.05 | 4.67 | 4.47 | 4.77 | 5 |
| 2048 | 3.98 | 3.72 | 2.74 | 5.85 | 6.09 | 5.70 | 6.33 | 5 |
| 8192 | 11.94 | 10.62 | 7.52 | 19.86 | 12.85 | 11.48 | 14.39 | 5 |
| 32768 | 35.44 | 28.84 | 24.62 | 66.01 | 35.53 | 32.59 | 38.47 | 5 |
| 131072 | 228.30 | 202.35 | 166.45 | 362.06 | 121.43 | 117.78 | 126.97 | 5 |
| 524288 | 474.30 | 460.29 | 357.35 | 633.20 | 531.25 | 520.20 | 538.27 | 5 |
| 2097152 | 1879.08 | 1817.54 | 1675.09 | 2299.35 | 2011.46 | 1726.77 | 2090.06 | 5 |
| 8388608 | 20500.84 | 21256.90 | 14834.10 | 28584.20 | 3686.22 | 3167.11 | 3845.38 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2655.80 | 2652.00 | 2492.00 | 2919.00 | 5 |
| Boolean.BatchBoolean | 2.40 | 2.00 | 2.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 1.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.80 | 2.00 | 2.00 | 4.00 | 5 |
| Polygon.Zebra3 | 1253.20 | 1145.00 | 1115.00 | 1496.00 | 5 |

