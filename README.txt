# Fasta Data Processor

## Overview

The Fasta Data Processor is a C program that efficiently reads and processes FASTA data files. FASTA is a popular format used in genomics research to store protein sequence data. This program is designed to compare different data structures' efficiency in handling this type of data.

## Features

- Reads FASTA data files and processes the data efficiently.
- Compares the efficiency of different data structures for storing FASTA records.
- Reports the time taken to complete the processing and the average time over multiple runs.
- Demonstrates the usage of linked lists for managing FASTA data.

## Programs Included

The project includes the following programs:

1. **llloadonly**: Loads the data from the file without storing it.
2. **arraydouble**: Loads the data and stores all the records into an array.
3. **llheadonly**: Loads the data into a simple linked list.
4. **llheadtail**: Loads the data into a linked list with a pointer to both the head and tail.

## Getting Started

To compile and run the program, follow these steps:

1. Clone this repository to your local machine.
2. Compile the C program using the provided Makefile.
  
make

3. Run the desired program with the following command line arguments:

./program_name -R <REPEATS> /path/to/fasta_file

Replace `program_name` with the desired program (e.g., llloadonly), `<REPEATS>` with the number of times to repeat the load, and `/path/to/fasta_file` with the path to your FASTA data file.

## Options

- **-R \<REPEATS>**: Specify the number of times to repeat the load. The reported time will be the average time over these runs.

## Example Usage

Run the "llheadtail" version of the linked list code five times and report the results:

./llheadtail -R 5 /path/to/fasta_file


## Notes

- When growing arrays, a common strategy is to double the allocation size when the array is not big enough, which may result in some wasted space.

## Author

Gali Polyak




