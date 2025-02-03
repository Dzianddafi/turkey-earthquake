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

## Traditional Machine Learning Model

![Screenshot 2025-02-03 at 16 50 22](https://github.com/user-attachments/assets/5d864c2a-07dd-4e7a-b1c6-fdeda9eb0789)

I used traditional machine learning model for this project where my ML goal is to cluster the earthquake data that are located near the East Anatolian Fault. On February 6th 2023,
a giant earthquake occured and it should have produced a plenty much data on its region. Thus, a high density data should have been made after the earthquake. I Used 3 different
algos at first and I figure out that DBSCAN worked better than the others to cluster a such high density kind of data.

![Screenshot 2025-02-03 at 17 02 23](https://github.com/user-attachments/assets/4e8afc48-7cfd-40bc-99f3-7abb71da4787)
![Screenshot 2025-02-03 at 17 02 49](https://github.com/user-attachments/assets/c2657d7f-2789-4077-b565-72046c2bba83)
![Screenshot 2025-02-03 at 17 03 49](https://github.com/user-attachments/assets/8064ff8f-0ba9-454e-8120-d8de59090930)

