#cross validation

cross validation allows us to compare different ML methods and get a sense of how well
they will work in practice
we use cross validation because we need generalization of our model

types of cross val methods-
non-exhaustive tech
	hold out
	k fold
	stratified k fold
exhaustive tech(this involve learn and test on all possible ways to divide original data)
	leave one out cross val
	leave P out cross val

but how we know that first 75% data for training and last 25% for testing is the best way
to divide the data. or using middle one or last one
cross validation uses them all and summarizes the result

when we divide the data into 4 blocks and use one by one for testing and other for training
then combine the resukt is called Four-Fold cross validation.
no. of blocks can be arbitary


in extreme case, we call each individual row as one block, this is Leave One Out Cross
Validation

in practice divide the data into 10 blocks and do the same, it is called Ten-fold cross
validation


we can use 10 fold cross validation to help find best value for tuning parameter



Hold Out method-
this is evaluation method basically

divide data into training and test data (two disjoint sets)
and do model building on training data and evalation of metrics on test data.
if more training data then model induced good
if more test data then metric evaluation good

disadv is that if training contain only +ve then problem as model will learn +ve labels only
	and over presentation and under presentation of classes in training and test data, 	means unequal distribution of +ve and -ve


K-Fold Cross Validation-
divide data in k blocks and in ith iteration use ith bloack as test and other as training
build models for all and then combine the result

stratified kfold is like divide the data into folds having all representation of classes
so it is better than k fold mwthods



leave one out cross validation-
in this first record or row is taken as test data and other for training then 2nd as test
and remainig as training and so on and combine the full result after doing this for entire
dataset, but we can work this if there are like 1000 rows but if 1 million then difficult
when not to use this-
dataset huge
computational resource limited
when have lot of parameters to test(like depth, estimators... in tress tech)

disadv is low bias
	and outdated, not used now



