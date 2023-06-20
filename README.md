# abasequence
abasequence: Coding ABA patterns for sequence data
abasequence

The `abasequence` R package provides functions for analyzing and manipulating sequential data based on specific coding rules. 
It allows users to perform various operations on sequences, such as counting events, generating codes, identifying ABA patterns, and calculating the length of consecutive ABA-coded sequences.

Installation
------------
You can install `abasequence` from GitHub using the `devtools` package:

```R
devtools::install_github("yourusername/abasequence")
abasequence

To use the abasequence package, first load it into your R session:
library(abasequence)

The package provides several functions:

count_events: Count the number of times each event occurs in a sequence.
generate_codes: Generate codes based on specific rules for each three-element sequence.
create_is_aba: Create a dummy variable indicating whether a sequence represents ABA pattern or not.
generate_length_aba: Calculate the length of consecutive ABA-coded sequences.
generate_sequences: Generate sequential data from a vector.

**Examples**
Here are a few examples of how to use the functions in the abasequence package:

# Create a sequence of events
sequence <- c(3, 2, 3, 1, 4, 2, 4, 1, 4, 3, 2, 3)

# Count the events
event_counts <- count_events(sequence)

# Generate codes for each three-element sequence
codes <- generate_codes(sequence)

# Create a variable indicating ABA pattern
is_aba <- create_is_aba(codes)

# Calculate the length of consecutive ABA-coded sequences
length_aba <- generate_length_aba(is_aba)

# Generate sequences from a vector
sequences <- generate_sequences(sequence, 3)

Contributing
Contributions to abasequence are welcome. If you find any issues or have suggestions for improvements, please open an issue on the GitHub repository.

License
This project is licensed under the GNU Public License. See the LICENSE file for details.

Acknowledgements
This package was developed by Andrew Pilny (Associate Professor, University of Kentucky). We would like to thank the open-source community for their contributions and support.

