# SSH Mapping Data Challenge 2023
It contains the codes and the process that was carried out in the practice performed by **Ala Baccar** and **Joaquin Opazo**. The idea of this repository is to show the results as well as the procedure, implementations and codes used. 

This repository contains codes and sample notebooks for downloading and processing the SSH mapping data challenge.

The starter version can be found [here](https://github.com/CIA-Oceanix/4dvarnet-starter)

## Motivation
The goal is to investigate the best method for SSH (Sea Surface Height) reconstruction in different situations such as, varying the domain or testing in different periods of the year.
For this purpose, satellite observations were used to train the model and then to compare with the real data. 

### Data sequence

The dates of the totality of the information provided is between 01-07-2009 and 31-07-2010. So it was divided as follows for the models:
 
- Spin-up: 01-07-2009 to 31-07-2009
- Evaluation: 01-08-2009 to 01-10-2009
- Training: 01-01-2010 to 31-07-2010

**Add image**

## Leaderboard by Season
### January-February ("2010-01-01", "2010-02-28")
|Method|domain|lt|lx|mu|
|:----:|:--:|:-:|:--:|:--:|
|4DVarNet|gf|13.302|1.361|0.86964|
|Miost|gf|11.701|1.158|0.90162|

### April-May ("2010-04-01", "2010-05-31")
|Method|domain|lt|lx|mu|
|:----:|:--:|:-:|:--:|:--:|
|4DVarNet|gf|11.382|1.497 |0.86859|
|Miost|gf|10.21|1.435|0.89097|

### Octobre-Novembre ("2009-10-01", "2009-11-30")
|Method|domain|lt|lx|mu|
|:----:|:--:|:-:|:--:|:--:|
|4DVarNet|gf|11.168|1.655|0.8232|
|Miost|gf|10.035|1.655|0.90484|

## Leaderboard for the whole year
### Year (""2010-01-01", "2010-07-31"")
|Method|domain|mu|lt|lx|
|:----:|:--:|:-:|:--:|:--:|
|4DVarNet|gf	|13.414|1.202|0.83549|
|Miost|gf		|11.247|1.109|0.89896|
|4DVarNet|canaries	|20.759|0.101|0.94521|
|Miost|canaries		|25.314|0.252|0.95286|
|4DVarNet|osmosis	|14.396|1.037|0.96333|
|Miost|osmosis		|21.214|1.243|0.96494|
