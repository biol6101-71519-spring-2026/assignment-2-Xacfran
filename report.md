# Assignment 2


## Overall read quality
Neither reads, R1 or R2, pass the per base sequence quality. R2 seems the worst with a very steep decrease in Quality ($<$ 25) after 200bp. The fastqc report shows the whiskers of the boxplot for R2 with lower limits below 20 after base pair 160 and below a Phred score of 10 after base pair 200. R1 also shows a decrease in quality after base pair 200, but it is not as drastic, reaching Phred scores of 20. There also seems to be adapter sequence contamination in both reads.

## Mapping rates

Although at first sight it looks good because there is an equal amount of R1 and R2 reads, with 70% mapped, the real problem is that only 12.73% of the reads are properly paired. This means that reads are either mapped as singletons (0.63%) or not mapped at all., so, even though 70% mapped, paired reads didn't land in the same alignment region in the reference assembly.

## Quality concerns

The low mapping rate and the low percentage of properly paired reads suggest that the quality of the reads is poor, as detected especially in R2. The steep decrease in these reads after 200bp, and the presence of adapter contamination could be contributing to the poor mapping efficiency.