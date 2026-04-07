# Evaluation Results DeepTest Competition 2026

In total four tools competed against each other in benchmarking an LLM-based Manual Assistant for the Automotive Domain.
The overall ranking with the achieved scores is as follows:

| Tool     | Score | Place |
| -------- | ----- | ----- |
| ATLAS    | 0.599 | 1     |
| Exida    | 0.572 | 2     |
| Warnless | 0.515 | 3     |
| CRISP    | 0.444 | 4     |

In total two systems, one academic and one industrial have been tested with two different manuel configurations and LLMs. Following metrics have been applied:

- **Rate** represents the number of failures divided by the number of generated tests.
- **W** represents the number of warnings missed (normalized to the total number of possible warnings to be missed).
- **Cov** represents the failure coverage in percent approximated by assessing how many failure clusters are covered.

Detailed metrics results are as follows:

| Model      | Tool     | SUT1 -- Manuel1 (W) | Rate     | Cov      | S        | SUT1 -- Manuel2 (W) | Rate     | Cov      | S        | SUT2 -- Manuel1 (W) | Rate     | Cov      | S        | SUT2 -- Manuel2 (W) | Rate     | Cov      | S        |
| ---------- | -------- | ----------------------------- | -------- | -------- | -------- | ----------------------------- | -------- | -------- | -------- | ----------------------------- | -------- | -------- | -------- | ----------------------------- | -------- | -------- | -------- |
| GPT-4-mini | ATLAS    | **0.61**                      | 0.52     | 0.74     | 0.62     | **0.64**                      | 0.51     | 0.92     | **0.69** | **0.57**                      | 0.32     | **0.89** | **0.59** | **0.60**                      | 0.36     | 0.89     | **0.62** |
|            | CRISP    | 0.42                          | 0.32     | 0.50     | 0.42     | 0.46                          | 0.32     | 0.68     | 0.49     | 0.34                          | 0.15     | 0.61     | 0.37     | 0.35                          | 0.17     | 0.69     | 0.41     |
|            | Exida    | 0.39                          | **0.65** | 0.60     | 0.55     | 0.41                          | **0.67** | 0.91     | 0.66     | 0.34                          | **0.45** | 0.84     | 0.54     | 0.36                          | **0.45** | 0.85     | 0.55     |
|            | Random   | 0.49                          | 0.35     | **0.79** | 0.54     | 0.51                          | 0.34     | **0.94** | 0.60     | 0.38                          | 0.23     | 0.88     | 0.50     | 0.40                          | 0.24     | **0.90** | 0.51     |
|            | Warnless | 0.51                          | 0.58     | 0.78     | **0.62** | 0.55                          | 0.59     | 0.86     | 0.67     | 0.36                          | 0.30     | 0.84     | 0.50     | 0.40                          | 0.32     | 0.86     | 0.53     |
| GPT-5-chat | ATLAS    | **0.61**                      | 0.48     | **0.89** | 0.66     | **0.64**                      | 0.59     | 0.86     | 0.69     | **0.33**                      | 0.31     | 0.66     | 0.43     | **0.32**                      | 0.31     | 0.83     | **0.49** |
|            | CRISP    | 0.45                          | 0.27     | 0.71     | 0.47     | 0.48                          | 0.31     | 0.65     | 0.48     | 0.26                          | 0.35     | **0.91** | **0.51** | 0.26                          | **0.38** | 0.60     | 0.41     |
|            | Exida    | 0.45                          | **0.73** | 0.87     | **0.68** | 0.49                          | **0.88** | 0.84     | **0.73** | 0.21                          | **0.37** | 0.60     | 0.40     | 0.20                          | 0.37     | 0.79     | 0.46     |
|            | Random   | 0.51                          | 0.30     | 0.89     | 0.56     | 0.58                          | 0.38     | **0.91** | 0.63     | 0.20                          | 0.20     | 0.67     | 0.36     | 0.21                          | 0.21     | **0.85** | 0.42     |
|            | Warnless | 0.54                          | 0.53     | 0.87     | 0.65     | 0.59                          | 0.68     | 0.86     | 0.71     | 0.18                          | 0.22     | 0.58     | 0.33     | 0.20                          | 0.25     | 0.81     | 0.42     |


The following results were achieved regarding the number of failures found:

| Algorithm | Total number of failures | Average number of failures per SUT |
| --------- | -------------- | ----------------------- |
| ATLAS     | 4547.66        | 568.46                  |
| CRISP     | 7191.17        | 898.90                  |
| Exida     | 4405.17        | 550.65                  |
| Warnless  | 6229.34        | 778.67                  |

We thank all participants for taking part in the competition.

Lev Sorokin,
Ivan Vasilev,
Samuele Pasini
