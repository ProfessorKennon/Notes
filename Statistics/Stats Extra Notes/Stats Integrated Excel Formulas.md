# Stats Integrated Excel Formulas


## Integrated Excel #3
=average(cells)
=median(cells)
=mode.sngl(cells)
=max(cells)
=min(cells)

Quartiles (you need to find first, second, third, or fourth so type 1,2,3, or 4)
=quartile.exc(cells, which quartile)

Percentiles (type in percentile you need. I.e. to find 20th percentile type 0.20)
=percentile(cells, percentile needed)

Interquartile Range (IQR) = Q3 - Q1
Lower Limit Bound = Q1 - 1.5*IQR
Upper Limit Bound = Q3 +1.5*IQR

Midrange:
=(MAX(cells) + MIN(cells)) / 2

Standard deviation (pick sample or population):
=stdev.s(cells) 
=stdev.p(cells)
=range(cells)
### 
Question #4
Z-Score (autofill)

Stats Formula: 
![4117D765-E454-4D53-B23F-6ACE4DA74847](images/4117D765-E454-4D53-B23F-6ACE4DA74847.png)
Excel Formula:
=(B17-$C$12)/$C$13

-You then can use auto fill and drag down (little box in the bottom left hand corner when you click on the cell)
-The $ lock that cell in place.  Now the mean and standard deviation do not change when you drag it down.



## Integrated Excel #4

Permutations and Combination:
=PERMUT(cells)
=COMBIN(cells)

![6B9E5FD4-DDDF-448C-9260-433DE64A2248](images/6B9E5FD4-DDDF-448C-9260-433DE64A2248.heic)

## Integrated Excel #5

Binomial:
=binomial.dist(# of success, # of trials, probability of success as decimal, FALSE)

=binomial.dist.range(# of trials, probability of success, lower range #, higher range number  # )

The numbers for my problem #1: 
Probability of success: 39%
Number of trials: 5
![5CB113F3-D5B0-4433-9290-D02A47DD3DB0](images/5CB113F3-D5B0-4433-9290-D02A47DD3DB0.png)
![C2397A10-D3ED-48FB-90BE-1CF257303AF3](images/C2397A10-D3ED-48FB-90BE-1CF257303AF3.heic)

![C68C187D-75FE-480B-98FE-2E63634056B1](images/C68C187D-75FE-480B-98FE-2E63634056B1.heic)


## Integrated Excel #6
=correl(highlight one column, highlight the other column)

## 

Integrated Excel #7

![33BB4192-5D2E-4EBD-88F9-869192AA52E3](images/33BB4192-5D2E-4EBD-88F9-869192AA52E3.png)
## Integrated Excel #8

![E39456CE-2CA2-4A39-8FE8-5D895184AD39](images/E39456CE-2CA2-4A39-8FE8-5D895184AD39.png)

## 
Integrated Excel #9

#1
Row 9: Null is always =
Row 10: Alternative you have to read the problem, should be < or > or =/=

Row 15-27 is probably always going to be yes on all of them because if there is a no you can’t do the problem

Row 34-37:
Critical Value:
	If < 			=NORM.S.INV(B4)		
	If > 			=-NORM.S.INV(B4)		
	If =/=			=-NORM.S.INV(B4/2)

Sample Proportion (p-hat): G4/B5

Test Statistic: 		=(B35-G5)/SQRT((G5*(1-G5))/B5)
![58A018E5-A869-45C2-BEEF-215E49913118](images/58A018E5-A869-45C2-BEEF-215E49913118.jpeg)

P-Value:
	If < 			= NORM.S.DIST(B36,TRUE)				Gives you to the left
	If > 			=1-NORM.S.DIST(B36,TRUE)			Gives you to the right
	If =/=			=2*NORM.S.DIST(B36,TRUE)			Gives you to the left then times 2 because it’s 2 tail



#2

Row 12: Null is always =
Row 13: Alternative you have to read the problem, should be < or > or =/=

Row 15: < or > is one tail, =/= is two tail

 
Row 21: =(B5-B7)/(F5/SQRT(B6))
![32570F24-FF1E-44C4-A8A3-1FD80DC166E7](images/32570F24-FF1E-44C4-A8A3-1FD80DC166E7.jpeg)

Row 30:
	Smaller Critical Value: =NORM.S.INV(F6/2)
	Larger Critical Value:  =-NORM.S.INV(F6/2) (or =-C30)

