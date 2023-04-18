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

# Program Testing Scenarios
## Program - 1 Linear Search

**Note: EP - Equivalence Partitioning and BVA - Boundary Value Analysis**


The following table lists the testing scenarios for the linearSearch program:

| Type | Tester Action and Input Data | Expected Outcome |
| --- | --- | --- |
| EP | A=[1,2,3,4],v=4 | 3 |
| EP | A=[1,2,3],v=4 | -1 |
| BVA | A=[], v=2 | -1 |
| BVA | A=[2], v=2 | 0 |
| BVA | A=[0], v=0 | 0 |
| BVA | A=[1, 2,...,9998, 9999], v=9999 | 9999 |

![image](https://user-images.githubusercontent.com/75672638/232803120-06726719-7785-4b41-9c96-805369078a17.png)


## Program - 2 Frequency of occurance

The following table lists the testing scenarios for the Frequency of occurance program:

| Type | Tester Action and Input Data | Expected Outcome |
| --- | --- | --- |
| EP | A=[1,2,3,4,3], V=4 | 2 |
| EP | A=[1,1,1,1], V=1 | 4 |
| EP | A=[1,2,3], V= 'x' | Invalid input |
| EP | A=[1,2,3], V= null | Invalid input |
| BVA | A=[], V=2 | 0 (Invalid Input) |
| BVA | A=[-2147483648, 1, 2, 3], V= -2147483648 | 1 |
| BVA | A=[2,2,2], V=2 | 3 |

![image](https://user-images.githubusercontent.com/75672638/232805588-34a9bb89-04a1-471b-8cd4-a5f48ab07d55.png)

## Program - 3 Binary Search

The following table lists the testing scenarios for the Binary Search program:

| Type | Tester Action and Input Data | Expected Outcome |
| --- | --- | --- |
| EP | A=[1,2,3,4,5], V=3 | 3 |
| EP | A=[2,3,4], V=1 | -1 |
| EP | A=[1,2,3], V=5 | -1 |
| EP | A=[1,2,3,5], V=4 | -1 |
| BVA | A=[1,2,3], V=1 | 0 |
| BVA | A=[1,2,3], V=3 | 2 |
| BVA | A=[1,2,3], V=2 | 1 |

![image](https://user-images.githubusercontent.com/75672638/232845078-a6f49ae0-7d34-48d3-b1e4-2eedef8f84c4.png)



## Program - 4 Triangles

The following table lists the testing scenarios for the Triangles program:

| Type | Tester Action and Input Data | Expected Outcome |
| --- | --- | --- |
| EP | a = 5, b = 5, c = 5 | 0 |
| EP | a = 6, b = 6, c = 4 | 1 |
| EP | a = 3, b = 4, c = 5 | 2 |
| EP | a = 0, b = 0, c = 0 | 3 |
| EP | a=-1, b=-2, c=-3 | 3 |
| BVA | a = 1, b = 1, c = 1 | 0 |
| BVA | a = 2, b = 3, c = 4 | 2 |
| BVA | a = 1, b = 2, c = 3 | 3 |
| BVA | a = 3, b = 4, c = 7 | 3 |
| BVA | a = 6, b = 2, c = 5 | 2 |
| BVA | a = 8, b = 2, c = 5 | 3 |


![image](https://user-images.githubusercontent.com/75672638/232845205-0d08dbb6-7be3-4709-a912-297b68e5fbf9.png)

## Program - 5 Prefix of String

The following table lists the testing scenarios for the Prefix of the String program:

| Type | Tester Action and Input Data | Expected Outcome |
| --- | --- | --- |
| EP | s1 = "hello", s2 = "hello world" | true |
| EP | s1 = "apple", s2 = "apples" | true |
| EP | s1 = "", s2 = "hello" | false |
| EP | s1 = null, s2 = "hello world" | false |
| BVA | s1 = "", s2 = "" | true |
| BVA | s1 = "a", s2 = "a" | true |
| BVA | s1 = "abcdefghijklmnopqrstuvwxyz", s2 = "abcdefghijklmnopqrstuvwxyz" | true |
| BVA | s1 = null, s2 = null | false |
| BVA | s1 = "a", s2 = "b" | false |

![image](https://user-images.githubusercontent.com/75672638/232845283-d9178a77-be2f-40f5-9b86-5fd21ceab167.png)

## Program - 6 Triangle with different specifications

**(a)** Equivalence Classes: Isosceles, equilateral, scalene, invalid

**(b)** Equivalence Class 1:

* EQUILATERAL Triangle - Input: a = 5, b = 5, c = 5

Expected Output: EQUILATERAL

* Equivalence Class 2: ISOSCELES Triangle - Input: a = 6, b = 6, c = 4

Expected Output: ISOSCELES

* Equivalence Class 3: SCALENE Triangle - Input: a = 3, b = 4, c = 5

Expected Output: SCALENE 
* Equivalence Class 4: INVALID Triangle - Input: a = 0, b = 0, c = 0

Expected Output: INVALID

**(c)**

* Boundary Test Case 1: a + b = c - 1

Input: a = 2, b = 3, c = 4

Expected Output: INVALID

* Boundary Test Case 2: a + b = c + 1

Input: a = 3, b = 4, c = 7

Expected Output: INVALID

* Boundary Test Case 3: a = b + c - 1

Input: a = 6, b = 2, c = 5

Expected Output: INVALID

* Boundary Test Case 4: a = b + c

Input: a = 7, b = 2, c = 5

Expected Output: INVALID

* Boundary Test Case 5: a = b + c + 1

Input: a = 8, b = 2, c = 5

Expected Output: INVALID

**(d)**

* Boundary Test Case 1: a = c - 1, b<a+c

Input: a = 2, b = 1, c = 4

Expected Output: scalene

* Boundary Test Case 2: a = c + 1, b < a+c

Input: a = 8, b = 4, c = 7

Expected Output: scalene

**(e)**

* Boundary Test Case 1: a = b = c +1

Input: a = 2, b = 2, c = 1

Expected Output: isosceles

* Boundary Test Case 2: a = b = c - 1

Input: a = 6, b = 6, c = 7

Expected Output: isosceles

* Boundary Test Case 3: a + 1 = b = c - 1

Input: a = 2, b = 3, c = 4

Expected Output: scalene

**(f)**

Input: a = 3, b = 4, c = 5

Expected Output: scalene (valid right-angle triangle)

Input: a = 5, b = 4, c = 3

Expected Output: scalene (valid right-angle triangle)

Input: a = 6, b = 8, c = 10

Expected Output: scalene (valid right-angle triangle)

Input: a = 1, b = 1, c = 2

Expected Output: Invalid (invalid triangle)

Input: a = 3, b = 3, c = 3

Expected Output: equilateral (equilateral triangle)

Input: a = 4, b = 4, c = 7

Expected Output: isosceles (isosceles triangle)

**(g)**

Input: a = 1, b = 1, c = 1

Expected Output: EQUILATERAL

Input: a = 0, b = 0, c = 0

Expected Output: Invalid

**(h)**

Input: a = -1, b = -2, c = -3

Expected Output: Invalid

Input: a = -2, b = 4, c = 0

Expected output: Invalid

# Section B
