# hippocampal_network_for_TMS
Identifying the TMS cortical targets within the hippocampal network
Individualized transcranial magnetic stimulation (TMS) targeting using functional connectivity analysis of functional magnetic resonance imaging (fMRI) has been demonstrated to be advantageous in inducing neuroplasticity. However, how this approach can benefit modulating the episodic memory function supported by the hippocampal network remains elusive. 

Here, we use the resting-state fMRI data from a large cohort (Human Connectome Project) to reveal tentative TMS targets at cortical regions within the hippocampal network. We identified the average centroids of individualized targets at the medial prefrontal cortex (mPFC) and posterior parietal cortices (PPC) at [-10 50 10] and [-40 -70 31] in the left hemisphere, respectively.  The mPFC and PPC coordinate at the right hemispheres are [11 52 8] and [48 -60 24] in the right hemisphere, respectively. These coordinates can be reliably identified (>90% of individuals) when the seed time series in the functional connectivity analysis was derived from a weighted sum of time series at the cortex. Our results suggested candidate TMS target coordinates to improve the episodic memory function using TMS.

Reference:  Lee, H.-J. et al. _Hum. Brain Mapp._ (2025)

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


