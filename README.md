# NYC Parking Tickets
![NYC_Tickets](/Resources/NYC_Header.jpg)
# Overview

## Data 

* New York City parking violations from the whole year of 2017
* Data was produced by NYC Department of Finance
* The data was chosen based off of how versatile and multifacted it is

## The Machine Learning Model

### Random forest model 

We ran a random forest model to determine whether there was a correlation. Created a confusion matrix and listed the features by importance. 

![Screen Shot 2022-11-17 at 8 35 02 PM](https://user-images.githubusercontent.com/107375554/202616400-c55cde9d-3c84-4d7b-a2f3-c9ef5ee96a6d.png)

![Screen Shot 2022-11-17 at 11 21 28 PM](https://user-images.githubusercontent.com/107375554/202827594-c5d5f222-2a13-426d-8a96-1d9666daf891.png)

![Screen Shot 2022-11-17 at 7 35 51 PM](https://user-images.githubusercontent.com/107375554/202616442-7c7b26f1-3b3a-475f-8b2c-b9ef8aaa680f.png)


### Neural Network
We then decided to run a neural network to determine whether or not the type of ticket you get can be predicted by the area you are re in or the features of your car. 

Started by condensing as much information as possible. The column unique value counts looked as follows:

Before: 	
![Screen Shot 2022-11-17 at 10 22 13 PM](https://user-images.githubusercontent.com/107375554/202616485-c50ae944-ef97-450a-9b8a-7ecf846286e2.png)  After:
![Screen Shot 2022-11-17 at 10 46 57 PM](https://user-images.githubusercontent.com/107375554/202616507-b32cd312-a522-4c2b-9021-9a36b0f5c3d8.png)


Converted categorical data into numerical data using one-hot-encoder.

Used the Violation_Code column as the target variable / ‘y’

Built the following network:

![Screen Shot 2022-11-17 at 11 21 28 PM](https://user-images.githubusercontent.com/107375554/202616647-296d928c-9b3f-4005-b625-53e812c32275.png)


Unfortunately, we could not get an accuracy above 55%.

![Screen Shot 2022-11-17 at 11 20 55 PM](https://user-images.githubusercontent.com/107375554/202616664-d680507c-bc05-438d-8713-7ac1ace51796.png)


## Predictions

* Brighter vehicles get more tickets than duller colored cars 
* Lower income boroughs recieve more tickets than higher income boroughs 

## Database ERD
![NYC_Tickets](/Resources/ERD_SEG2.png)
</br>
## The Databases Inner Join
![NYC_Tickets](/Resources/NYC_InnerJoin.png)
</br>

# Link to Slides
https://docs.google.com/presentation/d/1ABV8zML5IUWkjDon-CexeNSiZA5Zqblzs9vv-W5tjfs/edit#slide=id.p

# Link to Tableau Dashboard
https://public.tableau.com/views/NYC_Parking_Tickets/Story1?:language=en-US&:display_count=n&:origin=viz_share_link

### Resources 
* Google Colab - we are currently using Google Colab to write all the code.
* Google Slides - this is used to create our presentation.
* Pandas - Pandas is used to read the files in Google colab.
* Tableau - Tableau will be used to create the dashboard and analyze the data visually. 

