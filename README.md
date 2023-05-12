### What is the data set we use?
the data  set ues is  Netflix movie and tv_show ratings prediction.
### what is the idae of the project? 
This project is an example of performing data mining techniques on a dataset useing  Python libraries and machine learning techniques to get models  to predict 
movie and tv_show ratings.
### what is the frist thing we do in  project?
After of course we improt the most important library like pandas,numpy,seaborn and matplotlib . We start in pre_processing.
### What is the problems we face in pre_processing and how we solve it?
**1**-we have so many Null values in colome Director,Cast and Country so if we drop the NUll value directly we lose more than half of the data,
so **to solve it** we replace all Null values to No Data using method replace in library numpy after we do this we drop the null value using 'dropna'.

**2**- we have duplicates values so **to solve it** we using 'drop_duplicates' method .                                                                                                                                    

**3**- we have coloum name 'Release_Date' to unify the date we using 'to_datetime' method, and we create new 3 coloumes year,month and day  to use it in visualizations.

**4**- we have most coloums in non numerical and most models need numerical data so **to solve it** we usine 'encoder.fit_transform()' method to fit the encoder on the column's values and transform them into numerical labels.

### what is next step after pre_processing?
After pre_processing we start to select the best algorithms in this dataset and apply it and calc Evaluate the model.
### What was the algorithms we used ?
we used two algorithms KMeans and Linear Regression , and Compar what is the best algorithms using silhouette_avg_kmeans (kmeans) and mse_lr (inear Regression) 

**if**  silhouette_avg_kmeans > 0 and silhouette_avg_kmeans > abs(mse_lr) If the condition is true, it means that the KMeans algorithm has a higher silhouette score and lower MSE compared to Linear Regression, suggesting that KMeans performs better. In this case, the code will print "KMeans is the better algorithm".

**else** the code will print "Linear Regression is the better algorithm".

after that we calc Evaluate the model (Mean Squared Error,R^2 Score) to Linear Regression and (Silhouette Score) to kmeans
### what is next step after select models and calc Evaluate?
After select models and calc Evaluate we visualizations using plot,sccoterplt....else 
