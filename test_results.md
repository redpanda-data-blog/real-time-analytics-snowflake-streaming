|   Test | Input Tuning                            | Output Tuning                              |   P99  Latency (s) | Msg/sec   |   MiB/sec |
|-------:|:----------------------------------------|:-------------------------------------------|-------------------:|:----------|----------:|
|      1 | batching.byte_size: 134217728 (128MiB)  | Max in flight: 64                          |              10.6  | 3,366,709 |    631.97 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|      2 | batching.byte_size: 157286400 (150 MiB) | Max in flight: 64                          |              10.8  | 3,596,364 |    675.08 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|      3 | batching.byte_size: 183500800 (175 MiB) | Max in flight: 64                          |              12.5  | 3,549,756 |    666.33 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|      4 | batching.byte_size: 157286400 (150 MiB) | Max in flight: 1000                        |              11.2  | 3,445,274 |    646.72 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|      5 | batching.byte_size: 157286400 (150 MiB) | Max in flight: 16                          |              11.1  | 3,571,449 |    670.4  |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|      6 | batching.byte_size: 157286400 (150 MiB) | Max in flight: 64                          |               9.37 | 3,655,669 |    686.21 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|        |                                         | build.parallelism: 4                       |                    |           |           |
|      7 | batching.byte_size: 157286400 (150 MiB) | Max in flight: 64                          |               9.05 | 3,732,055 |    700.55 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|        |                                         | build.parallelism: 7                       |                    |           |           |
|      8 | batching.byte_size: 157286400 (150 MiB) | Max in flight: 16                          |               9.16 | 3,681,007 |    690.97 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|        |                                         | build.parallelism: 7                       |                    |           |           |
|      9 | batching.byte_size: 157286400 (150 MiB) | Max in flight: 32                          |               8.63 | 3,667,048 |    688.35 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|        |                                         | build.parallelism: 7                       |                    |           |           |
|     10 | batching.byte_size: 183500800 (175 MiB) | Max in flight: 32                          |              11.9  | 3,534,908 |    663.54 |
|        |                                         | channel_prefix: "${REDPANDA_PIPELINE_ID}-" |                    |           |           |
|        |                                         | build.parallelism: 7                       |                    |           |           |