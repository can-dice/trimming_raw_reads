# Trimming Raw Reads Worksheet

<!--- Write name below --->
## Name: 

<!--- For this worksheet, answer the following questions--->

## Q1: What does "cleaning" your reads mean?
Answer:

### Q2: Open the script called "trim_raw_reads.sh". For every line that says ```insert description here```, replace that text with a description of what the line will do

### Q4: Attach an image of the plot from fastqc showing the average base quality from your reads files
![before-trimming-PHRED-plot-1](./images/<plot-for-reads1>)
![before-trimming-PHRED-plot-1](./images/<plot-for-reads2>)

---

## The following questions pertain to your first fastp run (without altering the parameters)
### Q5: How many reads were there in the R1 file before filtering?
Answer:
### Q6: How many bases were there in the R1 file before filtering?
Answer:
### Q7: What proportion of bases were above PHRED score of 20 before filtering?
Answer: 
### Q8: What proportion of bases were above PHRED score of 30 before filtering?
Answer: 

### Q13: How many reads were there in the R2 file before filtering?
Answer:
### Q14: How many bases were there in the R2 file before filtering?
Answer:
### Q15: What proportion of bases were above PHRED score of 20 before filtering?
Answer: 
### Q16: What proportion of bases were above PHRED score of 30 before filtering?
Answer: 

### Q17: How many reads were there in the merged file after filtering?
Answer:
### Q18: How many bases were there in the merged file after filtering?
Answer:
### Q19: What proportion of bases in the merged file were above PHRED score of 20 after filtering?
Answer: 
### Q20: What proportion of bases in the merged file were above PHRED score of 30 after filtering?
Answer: 

### Q21: What is the difference between the merged and unmerged files (in principle, not quantitatively)?
Answer:
### Q22: Why are the unmerged files for R1 and R2 different lengths?
Answer:

---

## The following questions pertain to Remix 1 (the first time you change fastp parameters)
### Q23: What parameters did you change?
Answer: I changed the cut_window_size parameter. I increased it to 6. This increases the amount of bases in the sliding window. 
### Q24: How did you expect this to change the filtering results (be specific)?
Answer: I would expect this to remove more bases due to a larger window sizeand no change in mean quality. There could be a single base in the new window that decreases the mean below 20 causing them to be removed. This would happen before but it would be increased with a larger window.
### Q25: Explain the results. Did the change cause an effect that matched your expectations? Use information from the fastp output to explain.
Answer: There actually wasn't that much of a differences. The mean on the boxplots adjusted a little and the kmer content was different. It was not what I expected but it makes sense. I only changed the window by 2 bases. If I wanted to see what I expected I should have changed it by a larger amount.

---

## The following questions pertain to Remix 2 (the first time you change fastp parameters)
### Q26: What parameters did you change?
Answer: 
### Q27: How did you expect this to change the filtering results (be specific)?
Answer: 
### Q28: Explain the results. Did the change cause an effect that matched your expectations? Use information from the fastp output to explain.
Answer: 

