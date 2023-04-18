# Lab7_202001257

## Name: Prarthee Desai

## Id: 202001257
# Section A
# Program for Determining the Previous Date

This program takes a triple of day, month, and year as input and determines the previous date. The input ranges are as follows: 1 <= month <= 12, 1 <= day <= 31, and 1900 <= year <= 2015.

## Test Cases

The following table lists the equivalence class test cases for the program:

| Test Case | Input | Expected Output | 
| --- | --- | --- | 
| 1a | (1, 1, 1900) | Invalid date | 
| 1b | (31, 12, 2015) | 30/12/2015 | 
| 1c | (29, 2, 2000) | 28/02/2000 | 
| 1d | (28, 2, 2001) | 27/02/2001 | 
| 2a | (0, 1, 1900) | Invalid date | 
| 2b | (32, 12, 2015) | Invalid date | 
| 2c | (31, 13, 2000) | Invalid date | 
| 2d | ("1", "January", "1900") | Invalid date | 
| 3a | (29, 2, 2000) | 28/02/2000 | 
| 3b | (29, 2, 2004) | 28/02/2004 | 
| 3c | (29, 2, 2008) | 28/02/2008 | 
| 4a | (29, 2, 1900) | Invalid date | 
| 4b | (29, 2, 2001) | Invalid date | 
| 4c | (29, 2, 2015) | Invalid date | 
| 5a | (31, 1, 2000) | 30/01/2000 | 
| 5b | (30, 4, 2000) | 29/04/2000 | 
| 5c | (29, 2, 2000) | 28/02/2000 | 
| 6a | (1, 1, 1900) | Invalid date | 
| 6b | (1, 2, 2000) | 31/01/2000 | 
| 6c | (1, 3, 2001) | 28/02/2001 | 

## Equivalence Classes

The following tables list the partitions for the day, month, and year inputs:

### Day

| Partition ID | Range | Status | 
| --- | --- | --- | 
| E1 | Between 1 and 28 | Valid | 
| E2 | Less than 1 | Invalid | 
| E3 | Greater than 31 | Invalid | 
| E4 | Equals 30 | Valid | 
| E5 | Equals 29 | Valid for leap year | 
| E6 | Equals 31 | Valid | 

### Month

| Partition ID | Range | Status | 
| --- | --- | --- | 
| E7 | Between 1 and 12 | Valid | 
| E8 | Less than 1 | Invalid | 
| E9 | Greater than 12 | Invalid | 

### Year

| Partition ID | Range | Status | 
| --- | --- | --- | 
| E10 | Between 1900 and 2015 | Valid | 
| E11 | Less than 1900 | Invalid | 
| E12 | Greater than 2015 | Invalid | 
