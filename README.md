# Project 1: Identifying Mutations in NGS Data

## Project Overview

Project One analyses Next Generation Sequencing Data (NGS) using Python, from 6 samples of fission yeast (Schizosaccharomyces pombe). The aim is to identify nucleotide mismatches by comparing sequencing reads against a reference DNA sequence, investigating the differences between untreated and treated samples. There are 6,000 sequencing reads in the dataset and each sample contains 1,000 reads. Samples 1,2 and 3 (treatment group) received genotoxic treatment and samples 4,5 and 6 remain untreated (control group). 

## Methods and Code Structure

This analysis is sorted into 5 main functions:
- `validate_read()` - checks if sequencing reads are valid and matches the expected sequence length and format of the nucleotide.
- `find_mutations()` - helps to  identify any mismatches between each read. It also finds the mismatches in the reference sequence.
- `analyse_reads()` - records mutation information and processes sequencing reads
- `summarise_samples()` - calculates the mismatch frequencies and summarises each sample's results. .
- `compare_positions()` - compares  the mutation frequencies in treatment and control groups. It assesses the statistical differences by using Welch’s t-test

To make the analysis organised and easy to test, the functions use Python data structures, loops, conditional statements and modular code. 

## How to Run the Project
The analysis  is shown as a Jupyter notebook and designed to run in Google Colab.

1. Open `Project_1_Sequence_Analysis.ipynb`.

2. Select the option to open the notebook in Google Colab.

3. Run the cells in order, top to bottom.

4. Review the outputs and final interpretation.

## Results
Higher mismatch percentages were seen in the treated samples compared to the control samples. 
In the treatment group, the mean mismatch percentage was 60.33% compared with 8.33% in the control group.
Welch’s t-test showed statistically significant differences at positions 97, 98 and 99.
These findings suggest an increased frequency of DNA mismatches after genotoxic treatment.

## Testing
- All functions were tested using the assessment tests.
- Additional test cases checked their behaviour with different inputs and edge cases.

## Tools
- Python
- Google Colab
- Jupyter Notebook





