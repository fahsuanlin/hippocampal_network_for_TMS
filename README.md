# hippocampal_network_for_TMS
Identifying the TMS cortical targets within the hippocampal network
Individualized transcranial magnetic stimulation (TMS) targeting using functional connectivity analysis of functional magnetic resonance imaging (fMRI) has been demonstrated to be advantageous in inducing neuroplasticity. However, how this approach can benefit modulating the episodic memory function supported by the hippocampal network remains elusive. 

Here, we use the resting-state fMRI data from a large cohort (Human Connectome Project) to reveal tentative TMS targets at cortical regions within the hippocampal network. We identified the average centroids of individualized targets at the medial prefrontal cortex (mPFC) and posterior parietal cortices (PPC) at [-10 50 10] and [-40 -70 31] in the left hemisphere, respectively.  The mPFC and PPC coordinate at the right hemispheres are [11 52 8] and [48 -60 24] in the right hemisphere, respectively. These coordinates can be reliably identified (>90% of individuals) when the seed time series in the functional connectivity analysis was derived from a weighted sum of time series at the cortex. Our results suggested candidate TMS target coordinates to improve the episodic memory function using TMS.

This is a public respository for the paper to be published.

##
Left hemisphere

| Condition | mPFC_X | mPFC_Y | mPFC_Z | mPFC_mean | mPFC_std | mPFC_median | mPFC_IQR | PPC_X | PPC_Y | PPC_Z | PPC_mean | PPC_std | PPC_median | PPC_IQR |
|-----------|--------|--------|--------|-----------|----------|-------------|----------|-------|-------|-------|----------|---------|------------|---------|
| atlas     | 0      | 62     | 4      | 18.1      | 1.5      | 17.9        | 1.8      | -42   | -64   | 48    | 18.9     | 4.2     | 18.2       | 5.8     |
| grp FC    | -9     | 53     | -2     | 11.1      | 3.1      | 11.2        | 1.5      | -41   | -69   | 33    | 6.2      | 2.9     | 5.7        | 4.4     |
| ind FC    | -10    | 49     | 7      | 3.4       | 2.3      | 2.8         | 2.6      | -40   | -67   | 30    | 4.8      | 2.6     | 4.4        | 3.6     |

Right hemisphere

| Condition | mPFC_X | mPFC_Y | mPFC_Z | mPFC_mean | mPFC_std | mPFC_median | mPFC_IQR | PPC_X | PPC_Y | PPC_Z | PPC_mean | PPC_std | PPC_median | PPC_IQR |
|-----------|--------|--------|--------|-----------|----------|-------------|----------|-------|-------|-------|----------|---------|------------|---------|
| atlas     | 0      | 62     | 4      | 17.8      | 1.7      | 17.7        | 1.7      | 40    | -66   | 44    | 21.8     | 4.6     | 21.6       | 5.7     |
| grp FC    | 10     | 56     | 2      | 8.2       | 2.4      | 7.9         | 2.3      | 45    | -60   | 27    | 5.8      | 2.9     | 5.1        | 4.0     |
| ind FC    | 12     | 50     | 4      | 4.2       | 2.9      | 3.5         | 3.3      | 46    | -59   | 25    | 5.2      | 2.7     | 4.8        | 3.7     |


##

 <br><br><br>     |                             |        | MNI coordinate | distance to target (mm) | MNI coordinate | distance to target (mm) |
| ---------------- | --------------------------- | ------ | -------------- | ----------------------- | -------------- | ----------------------- |
|                  | Seed time course definition | target | X              | Y                       | Z              | mean                    | std | median | iqr | X | Y | Z | mean | std | median | iqr |
| left hemisphere  | seedmap                     | atlas  | 0              | 62                      | 4              | 17.8                    | 1.7 | 17.6 | 2.0 | \-42 | \-64 | 48 | 18.5 | 4.7 | 18.0 | 6.2 |
| grp FC           | \-9                         | 54     | 1              | 11.3                    | 3.1            | 11.1                    | 2.0 | \-41 | \-72 | 34 | 6.4 | 2.9 | 5.9 | 4.3 |
| ind FC           | \-10                        | 50     | 10             | 3.6                     | 2.5            | 2.9                     | 2.8 | \-40 | \-70 | 31 | 5.0 | 2.7 | 4.6 | 3.7 |
| Seed             | atlas                       | 0      | 62             | 4                       | 18.2           | 2.0                     | 18.1 | 2.1 | \-42 | \-64 | 48 | 19.2 | 5.1 | 18.5 | 7.6 |
| grp FC           | \-9                         | 54     | 0              | 11.6                    | 3.6            | 11.6                    | 2.5 | \-41 | \-72 | 34 | 7.0 | 3.4 | 6.5 | 5.0 |
| ind FC           | \-10                        | 50     | 9              | 4.5                     | 3.3            | 3.7                     | 3.7 | \-39 | \-70 | 30 | 5.5 | 3.0 | 5.0 | 4.1 |
| right hemisphere | seedmap                     | atlas  | 0              | 62                      | 4              | 16.4                    | 1.9 | 16.2 | 2.0 | 40 | \-66 | 44 | 22.2 | 4.5 | 21.9 | 5.8 |
| grp FC           | 10                          | 59     | 6              | 8.7                     | 2.5            | 8.3                     | 2.3 | 48 | \-62 | 26 | 5.8 | 3.1 | 5.0 | 4.3 |
| ind FC           | 11                          | 52     | 8              | 4.4                     | 3.0            | 3.7                     | 3.5 | 48 | \-60 | 24 | 5.3 | 2.8 | 5.0 | 3.8 |
| Seed             | atlas                       | 0      | 62             | 4                       | 17.1           | 2.5                     | 16.7 | 2.4 | 40 | \-66 | 44 | 23.0 | 5.4 | 22.5 | 6.7 |
| grp FC           | 10                          | 59     | 5              | 9.9                     | 3.4            | 9.1                     | 3.1 | 47 | \-62 | 26 | 7.0 | 3.8 | 6.0 | 5.1 |
| ind FC           | 11                          | 51     | 6              | 5.6                     | 3.8            | 4.6                     | 4.3 | 48 | \-59 | 24 | 6.1 | 3.3 | 5.5 | 4.5 |
