The data set that we ues is  Netflix movie and tv_show ratings prediction.

This project is an example of performing data mining techniques on a dataset useing  Python libraries and machine learning techniques to get models  to predict 
movie and tv_show ratings.

we love the moves and we want to make project for it so we work in this data set

After of course we improt the most important library like pandas,numpy,seaborn and matplotlib . We start in pre_processing.

###  the problems we face in pre_processing and how we solve it.

**1**-we have so many Null values in colome Director,Cast and Country so if we drop the NUll value directly we lose more than half of the data,
so **to solve it** we replace all Null values to No Data using method replace in library numpy after we do this we drop the null value using 'dropna'.

**2**- we have duplicates values so **to solve it** we using 'drop_duplicates' method .                                                                                                                                    

**3**- we have coloum name 'Release_Date' to unify the date we using 'to_datetime' method, and we create new 3 coloumes year,month and day  to use it in visualizations.

**4**- we have most coloums in non numerical and most models need numerical data so **to solve it** we usine 'encoder.fit_transform()' method to fit the encoder on the column's values and transform them into numerical labels.

###The next step after pre_processing

After pre_processing we start to select the best algorithms in this dataset and apply it and calc Evaluate the model.

### The algorithms we used .
we used two algorithms Classification and Natural Language Processing (NLP) , and Compar what is the best algorithms using (accuracy for classification , accuracy Natural Language Processing)  

**if**  accuracy for classification > accuracy Natural Language Processing: If the condition is true, it means that the classification algorithm  performs better. In this case, the code will print "classification is the better algorithm".

**else** the code will print Natural Language Processing is the better algorithm".

after that we calc Evaluate the model (Mean Squared Error,R^2 Score) to classificationand  (Mean Squared Error,R^2 Score) to Natural Language Processing
### The  next step after select models and calc Evaluate.
After select models and calc Evaluate we visualizations using plot,sccoterplt....else 

### some visualizations and what we conclusion.

<img width="235" alt="66666666666" src="https://github.com/0Ahmed2003/project_datamining/assets/121387438/f189762f-c2d4-4c86-8c14-a289794f0307">
<img width="236" alt="555555555" src="https://github.com/0Ahmed2003/project_datamining/assets/121387438/d8243f1a-91ff-4b98-bea7-fed56d981cde">

we conclused 2019 is the most year that moves has Released and
we conclused 8 is the most Rating in moves 

 <img width="279" alt="image" src="https://github.com/0Ahmed2003/project_datamining/assets/121387438/0cae882e-409a-4f92-834d-387b88a52ff5">
 
 we conclused the moves (69.1%) is more that TV_Show (30.9%)

