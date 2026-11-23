# v2
This folder contains the same data as v1, but with the following corrections made to improve reproducibility. 

## Change Log
Changes made to the Excel sheets 
1. In `trainingData.xlsx` (`DCNs` sheet): swapped the DCN values for n-hexadecane and n-dodecane (corrected to 100.3 and 73.5), and reordered the alkane rows by ascending chain length.
1. Fixed a typo by renaming `n-butocyclohexane` to `n-butylcyclohexane` throughout `trainingData.xlsx` and `validationData.xlsx`.
1. Removed the `1_Tesla_magnet` subfolder (preserved in v1) and three accidentally committed Excel lock files.
1. In `trainingData.xlsx` (`hydrocarbons` sheet): renamed column header `n-hexane` → `n-heptane` (header typo only; column data were always n-heptane, DCN 56, matching Table 1 and the features file).

## Known Issue
1. In `validationData.xlsx` (hydrocarbons sheet), the sample labelled n-heptane shows decay curves closer to the n-dodecane training data than to the n-heptane training data. Given the time elapsed since the measurement and the preliminary nature of this data exploration, we cannot be certain what was actually measured in this column. We recommend ignoring it in any future use of this dataset.
