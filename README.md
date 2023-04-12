# Lab-7_202001006

## Section-A

Test Cases
| ID | Day | Month | Year| Expected Output |
|----|-----|-------|-----|-----------------|
|  1 | 1   |  5    |2000 | 30-04-2000      |
|  2 | 2   |  2    |2005 | 01-02-2005      |
|  3 | 29  |  2    |2001 | Invalid |
|  4| 1 | 3 | 2001 | 28-2-2001|
|  5| 1 | 3 | 2000 | 29-2-2001|
| 6| 31| 4|2012| Invalid|
| 7| 1| 1| 2000| 31-12-1999|
|8| 31|12|2015| 30-12-2015|
| 9| 30| 4|2016| Invalid|
|10| 1|1|1994|Invalid|


### Equivalence Class
Day:<br />
|ID| class | validity |
|--|-------|----------|
|El| dd<1 |Invalid |
|E2 |1<=dd<=28| Valid|
|E3 |dd=31 |Valid |
|E4| dd=29 |Valid |
|ES |dd=30| Valid |
|E6| dd > 31| Invalid |

Month: <br />

|ID| class | validity |
|--|-------|----------|
|E7| mm<1 |Invalid |
|E8 |mm = 1,3,5,7,8,10,12(months with 31 days) | Valid|
|E9 |mm = 4,6,9,11(months with 30 days) |Valid |
|E10|mm = 2(month with either 28 or 29 days) |Valid |
|E11 |mm > 12| Invalid |

Year: <br/>
|ID| class | validity |
|--|-------|----------|
|E12| yy<1900 |Invalid |
|E13 | leap year 1900<=yy<=2015 | Valid|
|E14 |non leap year 1900<=yy<=2015  |Valid |
|E15 |yy > 2015 |Invalid |
