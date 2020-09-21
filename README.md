# EarthquakesPredict
This is the first ML project I did when I was a undergraduate student. It seems ridiculous after I learn more knowledge about ML.
# Brief Introduction of what these code do.
<img src="https://github.com/Demoom/EarthquakesPredict/tree/master/Image/P5.PNG" width="40%" height="40%">
## Data Pre-processing
Loading data.<br>
Finding some data unuseable, such as earthquake not coused by natural, and some wrong string data can't fitted by model.<br>
In order to put these data into, text data also have to be convert into numerical value.<br>

Have a view of all data.<br>
![image](https://github.com/Demoom/EarthquakesPredict/tree/master/Image/P1.PNG)<br>
It seems that there are a lot of null values, they needed to be filled.<br>
I use Pearson Correlation try to find relationship between these features. And use these relationships to fill null values with mean value or mode value or zero.<br>
![image](https://github.com/Demoom/EarthquakesPredict/tree/master/Image/P2.png)<br>
I also draw plot of two varibles try to find specific relationship between then and fill their null values with more appropriate values. However, I don't discover such kind of relationship.<br>
I drew a map of the world, and point every earthquake of my data.<br>
![image](https://github.com/Demoom/EarthquakesPredict/tree/master/Image/P4.PNG)<br>

## Train Model and Predict
After filling all null value, data can be put into model.<br>
I use LinearRegression and GaussianNB to predict longitude and latitude, use the first three data as a basis to predict the fourth data (after I learn a lot of knowledge of ML, I konw they are not effective model to use in this project).<br>
They have a result of very low accuracy, then I change the way I predict, I decide to predict which region will have earthquake next time.<br>
I use KMeans to classify these earthquake data to differernt calssed and draw another map of world to show the result.<br>
![image](https://github.com/Demoom/EarthquakesPredict/tree/master/Image/P5.PNG)<br>
Then predict the time and region of next earthquake, show it in map.<br>
![image](https://github.com/Demoom/EarthquakesPredict/tree/master/Image/P6.PNG)<br>
