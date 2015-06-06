# Algorithms for NASA Tournament Laboratory

## Banner Marathon Match

R script to automatically compute the disaggregated scores for all 1747 submissions for each of the over 2000 abstracts.

Each abstract has one or more annotations. Each annotation is a pair made by a position in the abstract and a label. A true positive is a correct annotation. A false positive is an annotation that misses either the position, or the label, or both. 

The output file contains the following information for each abstract and each submission:

1. *tot_labels* "The number of annotations to be identified"

2. *positions* "A string vector of length equal to the number of annotations to be identified with zeros and ones, where 1 indicates a true positive, and 0 a missing or false positive annotation"

3. *true_positives* "The number of correct annotations (i.e., the sum of ones in the positions)"

4. *total_positives* "The number of true positives plus the number of false positives"
