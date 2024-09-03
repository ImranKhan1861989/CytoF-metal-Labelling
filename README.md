Case Normalization: The script converts all column names to lowercase before comparing them with the provided label_mapping. This allows for matching labels irrespective of whether they are in uppercase, lowercase, or mixed case.

Flexible Mapping: The label_mapping dictionary should now contain the lowercase version of the metal labels as keys (e.g., 'cd111') and the unified labels as values (e.g., 'Cd111').

Handling Files: The script processes all specified CyTOF files, applies the label normalization, and saves the updated files to the specified output directory.

Example Usage:
Suppose you have two CyTOF files:

experiment1.csv with labels like Cd111, Pt195, and Pd102
experiment2.csv with labels like cd111, pt195, and pd102
You would run the script, and it would unify these labels across the two files, saving the updated versions in the unified_cytof_files directory.

This should make it easier to process the samples in a single batch, regardless of the capitalization differences.
