# A5-1-Encryption-Algorithm
Implementation of A5/1 Encryption Algorithm which is part of our Informations and Security Homework.

* <a href="#Task">Task</a> </br>
* <a href="#Description">Description</a> </br>

<a id= "Task" ></a>
## Task
This is the task given: 
```Implement the A5/1 algorithm. Suppose that, after a particular step, the values in the registers are
X = (x0, x1, . . . , x18) = (1010101010101010101)
Y = (y0, y1, . . . , y21) = (1100110011001100110011) 
Z = (z0, z1, . . . , z22) = (11100001111000011110000)

Generate and print the next 8 keystream bits. Print the contents of X, Y and Z after the 8 keystream bits have been generated.``` 

<a id= "Description" ></a>
## Description
A5/1 is a stream cipher used to provide over-the-air communication privacy in the GSM cellular telephone standard. It is one of seven algorithms which were specified for GSM use.[1] It was initially kept secret, but became public knowledge through leaks and reverse engineering. A number of serious weaknesses in the cipher have been identified.

A5/1 is based around a combination of three linear feedback shift registers (LFSRs) with irregular clocking. The three shift registers are specified as follows:

| LFSR | Lenght  | Feedback                                                            | Clocking | Tapped           |
| no.  | in bits | polynomial                                                          | bit      | bits             |     
|------|---------|---------------------------------------------------------------------|----------|------------------|
| 1    | 19      | x^{19}+x^{18}+x^{17}+x^{14}+1} x^{{19}}+x^{{18}}+x^{{17}}+x^{{14}}+1| 8        | 13, 16, 17, 18   |
| 2    | 22      | x^{22}+x^{21}+1} x^{{22}}+x^{{21}}+1                                | 10       | 20, 21           |
| 3    | 23      | x^{23}+x^{22}+x^{21}+x^{8}+1} x^{{23}}+x^{{22}}+x^{{21}}+x^{{8}}+1  | 10       | 10	7, 20, 21, 22| 


![A5/1](https://upload.wikimedia.org/wikipedia/commons/5/5e/A5-1_GSM_cipher.svg)
