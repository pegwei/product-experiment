# product-experiment
Ashton's 2019 Honours project on popularity bias in consumer choice based on [Powell et al. (2017)](../powell_paper.pdf).  
experiment_x folders contain code to run each experiment, data folder contains data for Exp 1-3. 
* For Exp 1-3, there were 33 trials (25 + 8 filler). 
* More-reviewed products had ~150 reviews and the less-reviewed product always had 125 less reviews.
* Participants rate preference for more-reviewed or less-reviewed product on a 6-point scale. 

## Experiment 1
Values for each trial is [here](../experiment_2/values/product_values_maindata_experiment1.csv).  

Between-s conditions:  
1. Explanation (explained vs. unexplained)  

Within-s conditions:  
1. More-reviewed product ratings (2.7, 3.1, 3.8, 4.2, 4.6)
2. Advantage (0.3, 0.1, 0, -0.1, -0.3) 

## Experiment 2
Values for each trial is [here](../experiment_2/values/product_values_experiment2.csv). Some filler trials different to Exp 1. 

Between-s conditions:  
1. Explanation (explained vs. unexplained)  

Within-s conditions:  
1. More-reviewed product ratings (2.7, 3.1, 3.8, 4.2, 4.6)
2. Advantage (0.9, 0.3, 0, -0.3, -0.9)

## Experiment 3
Values for each trial same as Exp 1. There were 2 x 33 trials. 

Within-s conditions:
1. Explanation (explained vs. unexplained) 
2. More-reviewed product ratings (2.7, 3.1, 3.8, 4.2, 4.6)
3. Advantage (0.3, 0.1, 0, -0.1, -0.3)

## Data
What do the headings in each data file mean? 
* subj_id: random subject id 
* demographics = gender, age, language, country
* turkcode: randomly generated 6-digit number, used by MTurkers to confirm HIT
* condition: explained or unexplained
* similarexp: whether participants have completed a previous experiment on MTurk similar to this 
* ratings = first number (e.g. 2.7) indicates rating for the more-reviewed product. Second number (e.g. 1) indicates rating advantage with 1=0.3, 2=0.1, 3=0, 4=-0.1, 5=-0.3. So 2.7_1 indicates the trial comparing a more-reviewed product (2.7) with a less-reviewed product (2.4). 
  - ratings 4-6 = preference for more-reviewed product
  - ratings 1-3 = preference for less-reviewed product
* filler trials = all trials with 'fil' compare filler trials, all trials with 'eq' means number of reviews were equal.  

There is also a data file containing 'dichotomised' ratings
 - 1 = prefers more-reviewed product
 - 0 = prefers less-reviewed product
