# CrossValidation

cross validation allows us to compare different ML methods and get a sense of how well
they will work in practice

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

