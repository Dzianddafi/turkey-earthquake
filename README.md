# Visualizing Earthquake Data with Python

The devastating earthquake that struck Turkey on February 6, 2023, had a magnitude of 7.8 and was centered in Nurdağı, near Gaziantep. The tremors caused massive destruction 
in Turkey and Syria, claiming the lives of more than 50,000 people and injuring tens of thousands of others.

Many buildings were destroyed, leaving residents in emergency conditions amidst the winter season. Relief efforts included rescue operations, distribution of food, water, and 
psychosocial support, carried out by various local and international organizations to help survivors cope with the trauma and challenges of life after the disaster.

![turkey eq drawio (1)](https://github.com/user-attachments/assets/26da24e8-a926-478a-9858-d993476e8ef1)

In this project, the dataset used came from USGS where we can find it easily on their website [https://www.usgs.gov/programs/earthquake-hazards]. The data that I used here
is earthquake data from January 1st 2020 until January 1st 2024 which located near Turkey and have a minimum magnitude of 5.0. The Anatolian Fault data that I used here is 
given by a friend of mine but it also available in Kaggle as of November 2024.

![Screenshot 2025-02-03 at 16 49 09](https://github.com/user-attachments/assets/79e2a862-e7fe-4417-819c-e5151aef44bc)

## Exploratory Data Analysis
In this section, a brief EDA is implemented to the data to see an introduction of the data that I used in this project

![Screenshot 2025-02-03 at 17 38 53](https://github.com/user-attachments/assets/b0712a98-f87b-4b24-a4f5-5f3cbf77e553)

### Key takeaways
The amount of earthquakes happened during February 6th 2023 to January 1st 2024 is 50 which presents 51.55% of the data being used in this project. Although the span of time is 
much shorter, the amount of earthquake that occured during this span of time ( under 1 year ) has already overcome the amount of earthquakes during Janurary 1st 2020 to 
February 6th 2023 ( over 3 years )

## Traditional Machine Learning Model

![Screenshot 2025-02-03 at 16 50 22](https://github.com/user-attachments/assets/5d864c2a-07dd-4e7a-b1c6-fdeda9eb0789)

I used traditional machine learning model for this project where my ML goal is to cluster the earthquake data that are located near the East Anatolian Fault. On February 6th 2023,
a giant earthquake occured and it should have produced a plenty much data on its region. Thus, a high density data should have been made after the earthquake. I Used 3 different
algos at first and I figure out that DBSCAN worked better than the others to cluster a such high density kind of data.

![Screenshot 2025-02-03 at 17 02 23](https://github.com/user-attachments/assets/4e8afc48-7cfd-40bc-99f3-7abb71da4787)
![Screenshot 2025-02-03 at 17 02 49](https://github.com/user-attachments/assets/c2657d7f-2789-4077-b565-72046c2bba83)
![Screenshot 2025-02-03 at 17 05 47](https://github.com/user-attachments/assets/7a5290af-adaa-4328-9781-d8617226a10d)

After finding out that DBSCAN works bettter, I test the epsilon number to see the maximum range that can be clustered as a high density data. I tested 1.3, 1.7, 1.9 for the epsilon
and it works the best for 1.7 as shown in these figures below.

![Screenshot 2025-02-03 at 17 08 54](https://github.com/user-attachments/assets/223ba3ca-c792-4aa8-97af-f88ba7566c9a)
![Screenshot 2025-02-03 at 17 09 13](https://github.com/user-attachments/assets/630d5506-f6f8-44ac-898e-4c6ff225df6e)

From figures above, we can see that epsilon 1.7 can involved the data inside the green marker (near the East Anatolian Fault) and left out the data inside the red marker 
(far from the East Anatolian Fault). Thus, epsilon 1.7 perform better that 1.3 and 1.9 that underfitted and overfitted respectively.

## Data Visualization


## Analysis
The analysis objective for this project is to find the moving trend of the earthquake

![Screenshot 2025-02-03 at 17 41 44](https://github.com/user-attachments/assets/eb823d17-50f7-470c-9d10-d03c9442a6de)

The figure above shows that from each data that is labeled by the ML, only 22.22% that occured before the earthquake on February 6th 2023. This conclude that 77.77% data that occured inside the high densed data could be produced by the earthquake since a main earthquake can have a following and still related to it.

![Screenshot 2025-02-03 at 17 42 48](https://github.com/user-attachments/assets/29cfa40a-c59e-4fd3-85a8-813d89bebf11)

The Figure above described the different location between before and after February 6th 2024. On the left side, we can see that almost every data produced located on the north-east side of the image and the right side described that earthquakes on and anfter February 6th located on the south-west side of the image. This trend can conclude that most likely, the earthquake in this area is moving from north-east to south-west of the image which is located near the East Anatolian Fault.

Figure below shows if the data that occured before and after the giant earthquake shown at the same time. This picture defined that not every earthquake  on the south-west side was labeled as the earthquake that happened on or after the giant earthquake on February 6th 2023.

![Screenshot 2025-02-03 at 17 52 41](https://github.com/user-attachments/assets/ae101036-3a4e-4f86-833c-2eff81830df1)

This marks as the end of the project, Thanks for looking at this project. Feel free to contact me regarding of this project in order to discuss or provide any further advice.
