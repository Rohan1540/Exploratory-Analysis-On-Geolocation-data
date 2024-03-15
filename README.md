![Screenshot 2024-03-15 232424](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/5100a1a7-f5d5-4bad-be06-ebc94343bffd)# Exploratory-Analysis-On-Geolocation-data
This project involves the use of K-Means Clustering to find the best accommodation for students in Hyderabad by classifying accommodation for incoming students on the basis of their preferences on amenities, budget and proximity to the location.

The Project has different stages which are mentioned in the flow diagram below:
![geolocation data flow diagram](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/ce99b0e5-ec3c-4404-afd9-519f30aed2a6)

The Approach for creation of the project would be as follows:
• Fetch Datasets from the relevant locations (Data Collection)
• Clean the Datasets to prepare them for analysis. (Data Cleaning via Pandas)
• Visualise the data using boxplots. (Using Matplotlib /Seaborn /Pandas)
• Fetch Geolocational Data from the Foursquare API. (REST APIs)
• Use K-Means Clustering to cluster the locations (Using ScikitLearn)
• Present findings on a map. (Using Folium/Seaborn)

Out of 70 different Columns selecting the most necessary data columns required for the analysis
![Screenshot (260)](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/a7fcb509-8ca2-4240-8839-be1c02b963fc)


A Box-plot graph can be helpful to look at distributed groups. It can tell us at glance where the population is concentrated, and how the outliers are as compare to the average object in the group.
![Screenshot (261)](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/0f69f9ec-77b4-4a52-9773-04ac211b02f7)

K Means Clustering will help us group locations based on the amenities located around them. For example, a location with a high amount of shops nearby will be labeled "Amenity Rich" while a location with less amenities will be labeled "Amenity Poor". Similar locations will be grouped (clustered) together.
![Screenshot (262)](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/6131a05c-3d39-486c-9719-913594ba3358)

Now since we have the optimal clusters then we would get access to the FourSquare API for the geolocation data which is necessary for plotting in the map because from there based upon the clusters we can extract the longitude and latitude as well as the type of the aminities provided in that particular sector of data.
![Screenshot 2024-03-15 231014](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/57fe076b-fc57-4ef1-8589-59fa29d9d1d3)

As from the above screen-shot we can observe the data flowing through the API and hence providing the data necessary for further operations, here the use of FourSquare V2 version of the API is used which is depreciated but somehow it worked for the project so the saying "IF IT WORKS THEN DONT TOUCH IT" helped me 😅, Now the data is formatted correctly for further processing so that the data which is not required is removed and we can get the valid data for the aminities.
![Screenshot 2024-03-15 231721](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/b949e1c5-1c85-4a4f-8b77-93ee48e1e23b)
![Screenshot 2024-03-15 231014](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/a7ce4afa-dd39-4bc5-8690-9214332355ff)
![Screenshot 2024-03-15 232121](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/35a8d159-74f8-4272-900d-40d4a0e7758f)

Now using the K-Means Clustering again and plotting the data on the map using the "Folium" Library
![Screenshot 2024-03-15 232424](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/89daba71-19b9-49e1-b34b-7dc6901d06f4)
![image](https://github.com/Rohan1540/Exploratory-Analysis-On-Geolocation-data/assets/96494363/f13fbf9d-b05d-4ed6-a3fb-967e8056a27f)

And there we have the data on the map which shows the places where it's beneficial for the students to live according to their budget and aminities provided👍.


