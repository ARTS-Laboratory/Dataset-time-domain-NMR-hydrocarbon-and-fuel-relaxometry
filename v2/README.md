# v2
This folder contains the same data as v1, but with the following corrections made to improve reproducibility. 

## Change Log
Changes made to the Excel sheets 
1. In `trainingData.xlsx` (`DCNs` sheet): swapped the DCN values for n-hexadecane and n-dodecane (corrected to 100.3 and 73.5), and reordered the alkane rows by ascending chain length.
1. Fixed a typo by renaming `n-butocyclohexane` to `n-butylcyclohexane` throughout `trainingData.xlsx` and `validationData.xlsx`.
1. Removed the `1_Tesla_magnet` subfolder (preserved in v1) and three accidentally committed Excel lock files.
1. In `trainingData.xlsx` (`hydrocarbons` sheet): renamed column header `n-hexane` → `n-heptane` (header typo only; column data were always n-heptane, DCN 56, matching Table 1 and the features file).

## Known Issue
1. In `validationData.xlsx` (hydrocarbons sheet), the curves labelled n-heptane show decay rates closely matching the n-dodecane training curves rather than the n-heptane training curves. These curves may have been acquired from a mislabelled sample. Users should treat this column with caution.
