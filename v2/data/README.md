# Data

This dataset was collected using a 0.645 Tesla magnet at 27.5 MHz. It contains a total of 161 T2 relaxation curves probed from 12 pure hydrocarbon and 17 jet fuel samples. The derived cetane number (DCN) of all samples is provided. 

All of the T2 relaxation data is provided in excel files. The first two sheets of the "trainingData" and "validationData" excel files contain hydrocarbon and jet fuel T2 data, where the first column is time (in seconds) and the remaining columns are T2 curves (in volts). The third sheet of the "trainingData" excel file summarizes the DCN of the samples. The code example.m shows how to read the data and plot relaxation curves using MATLAB. 

A note on amplitudes: initial signal amplitude varies with ambient temperature between acquisition days, so curves were amplitude-renormalized before export. Decay rate (and therefore T₂) is unaffected by this renormalization. Unfortunately, however, the specific renormalization procedure was not recorded. Absolute amplitudes should thus be treated as comparable in shape but not in absolute scale across samples or acquisition dates. 

## trainingData.xlsx
Three sheets: `hydrocarbons`, `jet fuels`, and `DCNs`.

## testData.xlsx
A single `jet fuels` sheet containing five acquisitions each of the two reference fuels CN40 (DCN 42.0) and CN50 (DCN 53.4).

## validationData.xlsx
Two sheets: `hydrocarbons` and `jet fuels`. Each holds five reprobes of five samples drawn from the training set, acquired on a later date than the training data. 
