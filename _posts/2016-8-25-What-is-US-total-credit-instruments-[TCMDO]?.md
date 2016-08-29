---
layout: post
title: What is the total amount of credit instruments in the US [TCMDO]?
---

**_v1.2_**

The short answer is that the number represents all of the [credit](http://hackeconomics.com/what-is-credit/) issued to consumers, corporations, and the government and is represented below:

<iframe src="//fred.stlouisfed.org/graph/graph-landing.php?g=6RPZ&width=670&height=475" scrolling="no" frameborder="0" style="overflow:hidden; width:670px; height:525px;" allowTransparency="true"></iframe>

That is, if you add up all of the debt incurred in the US for a particular point in time, you get this number. There is a way to look at (some) of the details of what makes up this number, however, this has a "through the looking glass" feel to it due to the rabbit holes you can go down looking at all of its components. The FRED series _Total Credit Market Debt Owed_ has a series code of FL894104005. The code reflects a line in a table contained in the Flow of Funds account. You can enter that number [here](https://www.federalreserve.gov/apps/fof/SeriesAnalyzer.aspx?s=FL894104005&t=) which returns the other series codes whose totals were used to calculate this number:

```
= + FL144104005 + FL154104005 + FL214104005 + FL314104005 + FL413065005 + FL264104005 + FL404104005 + FL614104005 + FL704104005 + FL674122005 + FL644104005 + FL543169373 + FL664104005 + FL734104005 + FL504104005 + FL513169333
```

After an email to the folks over at [FRED](http://hackeconomics.com/what-is-FRED/), unfortunately not all series in the flow of funds accounts are available in FRED. So, how about going into the Flow of funds account site itself? Well, it turns out that in 2015, the FR decided to discontinue the following table:

F.1 Total Credit Market Borrowing and Lending 1
Billions of dollars; quarterly figures are seasonally adjusted annual rates

Description	2009 
2010 
2011 
2012 
2013 
2014 
2014 
Q1	2014 
Q2	2014 
Q3	2014 
Q4	2015 
Q1	
Line
All sectors; credit market instruments; liability	-338.7	652.6	1113.2	1592.3	1953.1	2150.7	1547.0	2168.0	2318.8	2569.2	1130.3	1
Domestic nonfinancial sectors; credit market instruments; liability	1102.4	1405.4	1281.8	1823.0	1470.3	1723.0	1680.0	1399.4	1798.6	2013.9	1172.6	2
Households and nonprofit organizations; credit market instruments; liability	1.3	-154.0	-31.5	199.5	203.0	386.4	298.6	484.2	389.7	373.1	292.1	3
Nonfinancial corporate business; credit market instruments; liability	-358.7	-70.9	294.9	362.6	428.1	463.4	605.7	325.3	399.7	522.9	542.0	4
Nonfinancial noncorporate business; credit market instruments; liability	-97.1	-19.4	3.2	126.0	119.0	219.7	73.4	239.7	179.9	385.9	252.2	5
Federal government; credit market instruments; liability	1443.9	1580.2	1067.9	1140.2	759.1	667.1	741.0	314.4	913.1	700.0	-53.8	6
State and local governments, excluding employee retirement funds; credit market instruments; liability	113.0	69.5	-52.7	-5.3	-38.9	-13.7	-38.8	35.7	-83.7	32.2	140.2	7
Financial business; credit market instruments; liability	-1663.4	-901.8	-341.4	-419.3	213.9	271.7	-300.4	323.8	466.2	597.2	-340.7	8
U.S.-chartered depository institutions; credit market instruments; liability	-292.2	-217.6	-50.5	-110.8	-33.5	35.1	-25.8	106.3	35.8	24.0	-136.2	9
Foreign banking offices in the U.S.; bankers' acceptances; liability	0.0	0.0	0.0	0.0	0.0	0.0	0.0	0.0	0.0	0.0	0.0	10
Credit unions; FHLB advances; liability	-14.1	-0.4	-2.0	0.9	1.9	8.4	1.7	10.2	12.7	9.0	-2.0	11
Life insurance companies, general accounts; FHLB advances; liability	-6.6	-3.2	1.8	4.8	7.8	12.4	7.7	8.0	13.7	20.3	14.4	12
Government-sponsored enterprises; credit market instruments; liability	-518.4	-233.8	-187.2	-154.6	107.5	75.3	-355.5	156.9	142.5	357.3	-163.5	13
Agency-and GSE-backed mortgage pools; total mortgages; asset	458.3	186.9	165.3	132.2	132.4	75.3	77.4	27.8	83.4	112.6	-0.9	14
Issuers of asset-backed securities; total liabilities	-614.1	-413.9	-174.2	-145.1	-234.6	-68.4	-165.8	-90.5	-2.9	-14.3	-73.7	15
Finance companies; credit market instruments; liability	-156.2	-174.9	-13.5	-56.7	4.2	28.9	-24.5	11.6	48.0	80.2	62.8	16
Real estate investment trusts; credit market instruments; liability	-27.6	0.1	25.6	35.5	178.4	75.0	140.1	49.4	57.4	53.1	44.4	17
Security brokers and dealers; credit market instruments; liability	-49.7	36.9	-37.9	-1.7	22.2	11.5	41.3	-37.4	42.1	-0.1	-65.9	18
Holding companies; credit market instruments; liability	-8.0	-16.5	-16.5	-99.9	0.5	-8.3	12.9	4.0	-45.0	-5.2	-55.3	19
Funding corporations; credit market instruments; liability	-434.8	-65.3	-52.4	-23.9	27.0	26.5	-10.0	77.5	78.3	-39.7	35.2	20
Rest of the world; credit market instruments; liability	222.2	149.0	172.8	188.6	268.8	156.1	167.4	444.9	54.0	-42.0	298.4	21
All sectors; credit market instruments; liability	-338.7	652.6	1113.2	1592.3	1953.1	2150.7	1547.0	2168.0	2318.8	2569.2	1130.3	22
Domestic nonfinancial sectors; credit market instruments; asset	352.6	71.3	-265.6	-121.7	-512.9	-300.5	-769.1	-172.7	-168.8	-91.3	-377.3	23
Households and nonprofit organizations; credit market instruments; asset	70.5	-95.1	-207.9	-244.9	-568.8	-477.1	-932.3	-420.3	-267.5	-288.3	-797.4	24
Nonfinancial corporate business; credit market instruments; asset	10.2	2.6	-7.1	-12.8	-24.4	-16.7	-5.7	-11.5	-18.2	-31.3	33.3	25
Nonfinancial noncorporate business; credit market instruments; asset	-6.7	6.6	-4.7	1.8	2.7	4.9	1.9	5.3	3.8	8.6	6.5	26
Federal government; credit market instruments; asset	309.2	84.5	18.3	104.9	124.2	115.2	130.2	110.6	115.2	104.8	120.3	27
State and local governments, excluding employee retirement funds; credit market instruments; asset	-30.6	72.6	-64.2	29.3	-46.6	73.2	36.8	143.2	-2.1	114.9	260.0	28
Financial business; credit market instruments; asset	-807.8	-37.9	1141.3	1270.5	1914.8	1914.3	1812.0	1942.9	1943.5	1958.8	1147.9	29
Monetary authority; credit market instruments; asset	1001.6	271.5	376.5	34.5	1086.1	480.6	911.1	538.5	299.7	173.1	21.6	30
U.S.-chartered depository institutions; credit market instruments; asset	-280.4	-120.7	173.7	424.0	253.5	672.5	667.0	763.4	534.2	725.5	916.2	31
Foreign banking offices in the U.S.; credit market instruments; asset	-287.5	-24.4	42.5	5.8	-7.2	56.4	67.0	54.6	-3.0	106.9	65.7	32
Banks in U.S.-affiliated areas; credit market instruments; asset	-2.8	-19.3	-4.9	-0.1	0.3	-5.6	-0.3	-10.3	-7.0	-4.6	-16.3	33
Credit unions; credit market instruments; asset	34.1	24.9	38.6	47.0	50.2	60.2	48.5	75.6	82.0	34.8	52.2	34
Property-casualty insurance companies; credit market instruments; asset	33.3	3.9	36.2	1.0	30.9	15.8	-14.6	14.7	42.0	21.2	-15.1	35
Life insurance companies; credit market instruments; asset	139.8	151.6	125.3	74.3	77.4	99.7	117.7	128.9	76.9	75.3	142.2	36
Private pension funds; credit market instruments; asset	9.5	120.6	73.6	146.6	50.7	33.1	-8.2	78.8	45.5	16.3	51.1	37
Federal government retirement funds; credit market instruments; asset	7.4	10.9	25.6	15.4	9.4	16.9	6.1	9.4	20.6	31.6	-236.7	38
State and local government employee retirement funds; credit market instruments; asset	-83.1	22.4	7.4	3.3	79.5	35.1	18.3	35.5	83.3	3.0	2.5	39
Money market mutual funds; credit market instruments; asset	-619.9	-396.6	-9.8	-82.7	30.8	-120.8	-253.6	-356.5	150.4	-23.6	-102.0	40
Mutual funds; credit market instruments; asset	387.1	353.6	359.4	642.0	363.9	476.9	329.7	494.8	491.1	591.8	463.3	41
Closed-end funds; credit market instruments; asset	10.5	5.2	-1.7	11.2	13.6	-3.8	1.1	2.8	-10.6	-8.3	-1.4	42
Exchange-traded funds; credit market instruments; asset	46.0	29.7	46.1	52.3	12.2	51.0	43.8	48.2	24.4	87.6	77.1	43
Government-sponsored enterprises; credit market instruments; asset	-337.8	-288.4	-163.2	-189.4	59.8	69.6	-188.3	102.1	193.8	170.6	-199.0	44
Agency-and GSE-backed mortgage pools; total mortgages; asset	458.3	186.9	165.3	132.2	132.4	75.3	77.4	27.8	83.4	112.6	-0.9	45
Issuers of asset-backed securities; credit market instruments; asset	-579.5	-404.2	-170.0	-138.7	-229.2	-64.0	-160.0	-88.9	8.6	-15.6	-73.7	46
Finance companies; credit market instruments; asset	-214.9	-102.6	-44.4	-28.6	-19.0	13.8	-2.0	19.9	-5.4	42.6	26.8	47
Real estate investment trusts; credit market instruments; asset	-10.3	44.1	120.2	127.6	39.2	43.8	64.7	35.3	-1.1	76.5	-37.3	48
Security brokers and dealers; credit market instruments; asset	-192.1	32.2	5.7	89.1	-175.4	-81.0	-57.8	-28.8	-145.4	-92.0	53.5	49
Holding companies; credit market instruments;; asset	-16.0	22.1	3.1	-50.1	56.2	-11.1	-25.4	-8.1	36.3	-47.0	-32.0	50
Funding corporations; credit market instruments; asset	-311.3	38.7	-63.9	-46.4	-0.3	-0.2	169.9	5.1	-56.1	-119.6	-10.0	51
Rest of the world; credit market instruments; asset	116.5	619.2	237.4	443.5	551.1	536.9	504.1	397.8	544.1	701.7	359.7	52


Release dates | Announcements | Coded tables | Historical data | Technical Q&As
Current release | Screen reader | PDF (450 KB) | Data Download Program (DDP)
Statistical releases

Home | Economic research and data
Accessibility | Contact Us 
Last update: June 11, 2015



The description of each series:

```
+ FL144104005.Q	Nonfinancial business; debt securities and loans; liability
+ FL154104005.Q	Households and nonprofit organizations; debt securities and loans; liability
+ FL214104005.Q	State and local governments, excluding employee retirement funds; debt securities and loans; liability
+ FL314104005.Q	Federal government; debt securities and loans; liability
+ FL413065005.Q	Agency-and GSE-backed mortgage pools; total mortgages; asset
+ FL264104005.Q	Rest of the world; debt securities and loans; liability
+ FL404104005.Q	Government-sponsored enterprises; debt securities and loans; liability
+ FL614104005.Q	Finance companies; debt securities and loans; liability
+ FL704104005.Q	Private depository institutions; debt securities and loans; liability
+ FL674122005.Q	Issuers of asset-backed securities; debt securities; liability
+ FL644104005.Q	Real estate investment trusts; debt securities and loans; liability
+ FL543169373.Q	Life insurance companies, general accounts; FHLB advances; liability
+ FL664104005.Q	Security brokers and dealers; debt securities and loans; liability
+ FL734104005.Q	Holding companies; debt securities and loans; liability
+ FL504104005.Q	Funding corporations; debt securities and loans; liability
+ FL513169333.Q	Property-casualty insurance companies; FHLB advances; liability
```

Each of these series is made up of other series which you can peruse at your leisure [here](https://www.federalreserve.gov/apps/fof/SeriesAnalyzer.aspx?s=FL894104005&t=).

