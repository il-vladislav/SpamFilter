#### DESCRIPTION

Naive Bayes spam filtering with black/white lists and subject filtering. 

Filter is already trained on data sets, have dictionaries with spammers and hammers list, and list of spam/ham email subjects. Dictionaries is product of training on several training sets.
Filter uses Bayesian algorithm. 

#### PRIORITIES

1) Check  black list of spammers 
2) Check white list of "hammers"
3) Check subject spam/ham lists
4) Start Bayesian algorithm.

#### RESULTS

Student iliusvla earned 19.000(maximum ammount) points and is ranked on place 1.
#####  Data 1
|Rank |	tp |	tn 	|fp 	|fn 	|q
|---  |--- | ---    |  ---  |   --- | --- 
|1 (My) 	|461.000 	|153.000 	|0.000 	|0.000 	|1.000 
|2 	|459.000 	|153.000 	|0.000 	|2.000 	|0.997
|3 	|457.000 	|153.000 	|0.000 	|4.000 	|0.993
|4 	|461.000 	|152.000 	|1.000 	|0.000 	|0.984
|5 	|457.000 	|152.000 	|1.000 	|4.000 	|0.978

#####  Data 2
|Rank |	tp |	tn 	|fp 	|fn 	|q
|---  |--- | ---    |  ---  |   --- | --- 
|1(My) |	461.000 |	154.000 	|0.000 	|1.000 	|0.998
|2 	|462.000 	|153.000 	|1.000 	|0.000 	|0.984
|3 	|462.000 	|152.000 	|2.000 	|0.000 	|0.968
|4 	|459.000 	|151.000 	|3.000 	|3.000 	|0.949
|5 	|440.000 	|152.000 	|2.000 	|22.000 	|0.934 


#####  Data 3
|Rank |	tp |	tn 	|fp 	|fn 	|q
|---  |--- | ---    |  ---  |   --- | --- 
|1 (My)	|575.000 	|192.000 	|0.000 	|2.000 	|0.997
|2 	|567.000 	|192.000 	|0.000 	|10.000 	|0.987
|3 	|566.000 	|192.000 	|0.000 	|11.000 	|0.986
|4 	|562.000 	|192.000 	|0.000 	|15.000 	|0.980
|4 	|562.000 	|192.000 	|0.000 	|15.000 	|0.980 

#### SOME NOTES

While 425 million (as of June 28th, 2012) users use GMail, this Naive method is effective, but has one little problem: Service provider has to **generate dictionaries for every user individually (for best quality)**. 
To reduce required storage space there are several techniques: classify all mail to several categories and for every user classify every category as SPAM/HAM. Other technique is to classify all users to several categories 
and use one dictionary for every category. Analysis of best technique is beyond the scope this project. 


#### TO DO

Write some algorithm to make work check_common_spamers_pattern module (https://github.com/il-vladislav/SpamFilter/blob/master/common_spamers_pattern.py)
Try to ignore HTML code, when using Bayesian algorithm.
There is much thing to do, Machine Learning never stops...