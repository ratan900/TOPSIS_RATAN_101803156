# TOPSIS_RATAN_101803156
Project description
TOPSIS Package in Python
Submitted by: Ratan Kumar

Roll no: 101803156

UCS538

Concept of TOPSIS
TOPSIS is an acronym that stands for ‘Technique of Order Preference Similarity to the Ideal Solution’ and is a pretty straightforward MCDA method. As the name implies, the method is based on finding an ideal and an anti-ideal solution and comparing the distance of each one of the alternatives to those.

How to use
The package TOPSIS-Ratan-101803156 can be run though the command line as follows:

>> pip install TOPSIS-Ratan-101803156==0.3.0
>> python
>>>from topsis_analysis.topsispackage import topsis
>>>topsis("data.csv","1,1,1,2","+,+,-,+","output.csv")
Note:

Usages:

topsis( <InputDataFile> <Weights> <Impacts> <ResultFileName>)

Input File:

Input file contain three or more columns.
First column is the object/variable name (e.g. M1, M2, M3, M4……) .
From 2nd to last columns contain numeric values only.
Output File:

Result file contains all the columns of input file and two additional columns having TOPSIS SCORE and RANK
The output is created in the form of csv file and stored and also it is displayed.

The impacts given in the command line should be either ‘+’ or ‘–’ depending if you want to maximise the column parameter or minimise it.

Sample Input
Here is a sample set of data which can be used for the following package:

Model	Correlation	R2	RMSE	Accuracy
M1	0.79	0.62	1.25	60.89
M2	0.66	0.44	2.89	63.07
M3	0.56	0.31	1.57	62.87
M4	0.82	0.67	2.68	70.19
M5	0.75	0.56	1.3	80.39
Output of this sample input
The output that will be generated from the following input data will be:

Model	Correlation	R2	RMSE	Accuracy	Topsis Score	Rank
M1	0.79	0.62	1.25	60.89	0.6391330141342590	2.0
M2	0.66	0.44	2.89	63.07	0.21259182969277900	5.0
M3	0.56	0.31	1.57	62.87	0.4078456776130520	4.0
M4	0.82	0.67	2.68	70.19	0.5191532395007470	3.0
M5	0.75	0.56	1.3	80.39	0.8282665851935810	1.0
Here the ranks are given as rank 1 is the best solution according to the weights and impacts given and rank 5 is the worst solution.
