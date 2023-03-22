# Lab Report 5: Exploring Advanced Bash Commands

# Introduction

In this lab report, we will explore four useful Bash commands that are often used in Linux and Unix environments: `awk`, `sed`, `sort`, and `uniq`. These commands are designed for text processing and can be extremely useful when working with large data sets or text files. We will provide detailed explanations and examples to demonstrate the usefulness and capabilities of each command.

# 1. awk

The `awk` command is a text processing tool that allows for pattern scanning and processing. It is designed to efficiently perform operations on text files or data streams, such as filtering, transforming, or calculating values.

# Example:

Consider a file named `employees.txt` with the following content:

John,5000
Jane,6000
Tom,4500
Lisa,7000


To calculate the total salary of all employees, use the following command:

awk -F, '{sum+=$2} END {print sum}' employees.txt

# Explanation:

- `-F,` sets the field separator to a comma (,).
- `{sum+=$2}` adds the second field (salary) to the sum variable for each line.
- `END {print sum}` prints the total sum after processing all lines.

# Expected output:

22500


# 2. sed

The `sed` (stream editor) command is used for performing text transformations on an input stream (a file or input from a pipeline). It is particularly useful for searching and replacing text patterns within files.

# Example:

Consider a file named `fruits.txt` with the following content:

apple
banana
cherry
date


To replace 'cherry' with 'grape', use the following command:

sed 's/cherry/grape/' fruits.txt

# Explanation:

- `'s/cherry/grape/'` is a sed command that replaces the first occurrence of 'cherry' with 'grape' on each line.

# Expected output:

apple
banana
grape
date


# 3. sort

The `sort` command is used to sort lines of text files. It can be particularly useful when working with large files or when you need to quickly organize data in a specific order.

# Example:

Consider a file named `numbers.txt` with the following content:

4
2
8
5


To sort the numbers in descending order, use the following command:

sort -nr numbers.txt

# Explanation:

- `-nr` sorts the numbers in numerical and reverse order.

# Expected output:

8
5
4
2


# 4. uniq

The `uniq` command is used to remove duplicate lines from a sorted file. It can be helpful when working with large data sets to reduce redundancy and find unique data points.

# Example:

Consider a file named `colors.txt` with the following content:

red
green
red
blue
blue


To display unique colors, use the following command:

sort colors.txt | uniq

# Explanation:

- `sort colors.txt` sorts the file alphabetically.
- `uniq` removes duplicate lines from the sorted input.

# Expected output:

blue
green
red

# By Mohammed Azab/ChatGPT :)
