# Project 1: Identifying Mutations in NGS Data

## Project Overview

Project One analyses Next Generation Sequencing Data (NGS data) using python. The NGS data comes from 6 samples of fission yeast (Schizosaccharomyces pombe). The aim of the project is to identify the nucleotide mismatches by using a reference DNA sequence to compare sequencing reads against it, allowing us to investigate the differences between untreated and treated samples. There are six thousand sequencing reads in the dataset and each sample contains a thousand reads. Samples 1,2 and 3 are exposed to a genotoxic treatment so are the treated samples and the control samples are samples 4,5 and 6 as they remain untreated. 

## Methods and Code Structure

This analysis is sorted into 5 main functions:
- `validate_read()` - This checks is sequencing reads are valid and  match the expected sequence length and format of the nucleotide.
- `find_mutations()` - This helps to  identify any mismatches between each read. It also finds the mismatches in the reference sequence.
- `analyse_reads()` - This records the mutation information and processes sequencing reads
- `summarise_samples()` - This calculates the mismatch frequencies. It also summarises each sample's results. .
- `compare_positions()` - This looks at the mutation frequencies in treatment and control groups and compares them. It assess the statistical differences by using Welch’s t-test

To make the analysis easy to follow and test, these 5 functions use Python data structures, loops, conditional statements and modular code. 

## How to run the project
The analysis in project 1 is shown as a Jupyter notebook and designed to run in Google Colab.

1. Open `Project_1_Sequence_Analysis.ipynb`.

2. Select the option to open the notebook in Google Colab.

3. Run the cells in order, from top to bottom.

4. Review the outputs and final interpretation.

## Results
Higher mismatch percentages were seen in the treated samples compared to the control samples. 
In the treatment group, the average (mean) mismatch percentage was 60.33% compared with 8.33% in the control group.
Welch’s t-test showed statistically significant differences at positions 97, 98 and 99 between the groups. 
These findings suggest an increased frequency of DNA mismatches after the samples had been exposed to the genotoxic treatment.

## Testing
The functions in Project 1 were tested using all the given assessment tests. Additional test cases were also used to check their behaviour with different inputs and edge cases.

## Tools
- Python
- Google Colab
- Jupyter Notebook




