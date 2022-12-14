# NYC Parking Tickets
![NYC_Tickets](/Resources/NYC_Header.jpg)
# Overview

## Data 

* New York City parking violations from the whole year of 2017
* Data was produced by NYC Department of Finance
* The data was chosen based off of how versatile and multifacted it is

## Predictions

* Brighter vehicles get more tickets than duller colored cars 
* Lower income boroughs recieve more tickets than higher income boroughs 

## Database ERD
![NYC_Tickets](/Resources/ERD_SEG2.png)
</br>
## The Databases Inner Join
![NYC_Tickets](/Resources/NYC_InnerJoin.png)
## Vehicle Description Table
![NYC_Tickets](/Resources/Vehicle_desc.png)
</br>

## The Machine Learning Model

### Random forest model 

We ran a random forest model to determine whether there was a correlation. Created a confusion matrix and listed the features by importance. 

![Screen Shot 2022-11-17 at 8 35 02 PM](https://user-images.githubusercontent.com/107375554/202616400-c55cde9d-3c84-4d7b-a2f3-c9ef5ee96a6d.png)

![Screen Shot 2022-11-17 at 7 37 00 PM](https://user-images.githubusercontent.com/107375554/202827649-1dea37ef-72d4-4757-87b8-66f85535d7ab.png)

![Screen Shot 2022-11-17 at 7 35 51 PM](https://user-images.githubusercontent.com/107375554/202616442-7c7b26f1-3b3a-475f-8b2c-b9ef8aaa680f.png)


### Neural Network
We then decided to run a neural network to determine whether or not the type of ticket you get can be predicted by the area you are re in or the features of your car. 

Started by condensing as much information as possible. The column unique value counts looked as follows:

Before: 	
![Screen Shot 2022-11-17 at 10 22 13 PM](https://user-images.githubusercontent.com/107375554/202616485-c50ae944-ef97-450a-9b8a-7ecf846286e2.png)  After:
![Screen Shot 2022-11-17 at 10 46 57 PM](https://user-images.githubusercontent.com/107375554/202833364-317ee5e9-820d-4774-9d0f-6ac3e33e0ac3.png)



Converted categorical data into numerical data using one-hot-encoder.

Used the Violation_Code column as the target variable / ‘y’

Built the following network:

![Screen Shot 2022-11-17 at 11 21 28 PM](https://user-images.githubusercontent.com/107375554/202616647-296d928c-9b3f-4005-b625-53e812c32275.png)


Accuracy landed on 94%

<img width="570" alt="Screen Shot 2022-11-19 at 1 03 39 AM" src="https://user-images.githubusercontent.com/107375554/202837142-718765ad-0469-409d-805c-71249d2bdb2c.png">


The model was able to predict whether a car recieved a violation for street cleaning or speeding based on features. 



# Link to Slides
https://docs.google.com/presentation/d/1ABV8zML5IUWkjDon-CexeNSiZA5Zqblzs9vv-W5tjfs/edit#slide=id.p

# Link to Tableau Dashboard
https://public.tableau.com/views/NYC_Parking_Tickets/Story1?:language=en-US&:display_count=n&:origin=viz_share_link

### Resources 
* Google Colab - we are currently using Google Colab to write all the code.
* Google Slides - this is used to create our presentation.
* Pandas - Pandas is used to read the files in Google colab.
* Tableau - Tableau will be used to create the dashboard and analyze the data visually. 

