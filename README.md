# Applied Data science capstone Final project
This project will be mainly used for the Applied Data Science Capstone.

# 1. Introduction
Road accidents have become very common nowadays. As more and people are buying automobiles, the incidences of road accidents are just increasing day by day. 
As per WHO observatory data “Road traffic injuries are currently estimated to be the eighth leading cause of death across all age groups globally and are predicted to become the seventh leading cause of death by 2030”.

Analyzing an important array of factors, including weather conditions, speed, construction work, special events, traffic jams among others, an accurate prediction of the severity of the accidents can be performed.

These perceptions, could allow law enforcement bodies to allocate their resources more effectively in advance of potential accidents, preventing when and where a severe accident can occur as well as saving both, time and money. In addition, this knowledge of a severe accident situation can be warned to drivers so that they would drive more carefully or even change their route if it is possible or to hospital which could have set everything ready for a severe intervention in advance.

Governments should be highly interested in accurate predictions of the severity of an accident, in order to reduce the time of arrival and thus save a significant amount of people each year. Other attentive private companies could be investing in technologies aiming to improve road safeness.
  
 
Stakeholders:
 - Public Development Authority of Seattle

 - Car Drivers 
  
# 2. Data  
The data comes from Seattle car accident set. A comprehensive dataset of 194,673 accidents occuring between 2004-2020. The dataset has 38 columns describing the details of each accident including the weather conditions, collision type, date/time of accisent and location.

Location,Weather,Lighting, type of intersection, road conditions, collision condition, drunk and driver and other information described in the dataset.

The following features are selected for the prediction

INATTENTIONIND	- Whether or not accident was due to inattention (Y/N)

UNDERINFL	- Whether or not driver was in drug or alcohol (Y/N) 

WEATHER -	Weather condition

ROADCOND -	Condition of the road

LIGHTCOND -	Condition of the light

SPEEDING	- Whether or not Speeding was a factor (Y/N)


2.1 Pre-Processing

The models aim was to predict the severity of an accident, considering that, the variable of Severity Code was in the form of 1 (Property Damage Only) and 2 (Injury Collision).

Featured data are pre processed to convert into continuous data. Encode accident was due to attention with 0 as No and 1 as Yes. Road conditions can be segregate into dry, mushy and wet. Dry as 0, Mushy as 1 and Wet as 2. Ice,Standing Water and oil are similar to wet then it encode as 2. Snow/Slush and Sand/Mud/Dirt are encode as 1. There are few data with 'Others', So it encode as 'Unknown'. Weather conditions are encode like clear as 0, Overcast and Cloudy as 1, Windy as 2 and Rain as 3. Light conditions are encode like Light as 0, Medium as 1 and Dark asa 2. Encoding under the influence No as 0 and Yes as 1.

2.2 Cleaning

Data cleaning is the process of detecting and removing the inaccurate values from the data set. Here to remove Unknown or Other values from the data set. The entire process of cleansing data to reduce almost 10000 records which is having incorrect data.
