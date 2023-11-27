#  <img src="https://user-images.githubusercontent.com/71335808/167276461-662eb9f2-1c55-4c07-ac4e-791dc307a8a3.png" width="50" height="50"> Virtual Art Gallery Web App

## Introduction
Welcome to the virtual art gallery web application—a gateway to an immersive experience featuring over 80,000 2D artworks curated by the prestigious National Gallery of Art ([NGA](https://www.nga.gov/)). Our platform reimagines the conventional gallery visit by intertwining rich browsing capabilities with advanced data analysis tools. Users can seamlessly explore and appreciate these masterpieces from the comfort of their homes or any location, catering to both recreational and educational endeavors. The application offers a range of features, including artwork display, user-input keyword searches, selection filters, and robust data analysis functionalities. Our aspiration is to inspire individuals through this virtual journey, sparking an appreciation that may translate into physical visits to the NGA. We believe that this blended experience will enrich and elevate their perception of these extraordinary artworks.


## Features

### 1. Geographic Distribution of Artwork Origins
&nbsp;
![1](https://github.com/lingzix/Demo_gif/blob/main/Map.gif)

### 2. Search by selection filters
&nbsp;
![2](https://github.com/lingzix/Demo_gif/blob/main/Filter_search.gif)

### 3. Search by user-input keywords
&nbsp;
![3](https://github.com/lingzix/Demo_gif/blob/main/Keyword_search.gif)

### 4. Search by user height/birth year
&nbsp;
User can find artworks with the same height as themselves, or were created within the year they were born.

![4](https://github.com/lingzix/Demo_gif/blob/main/Naughty_search.gif)

### 5. Artwork Detail & Similar Artworks
&nbsp;
Detail is dynamically fetched from our database instance. A section of color palette is automatically generated based on each artwork for aesthetic inspirations. 4 similar artworks are recommended to users at the bottom. The algorithm utilizes the facts of shared artists/exhibition/style/theme/etc. Users can continue exploring similar artworks by a simple click.

![5](https://github.com/lingzix/Demo_gif/blob/main/Artwork_similar.gif)

### 6. Word cloud
&nbsp;
User can view frequency of each keyword by hovering the mouse over the cloud.

![6](https://github.com/lingzix/Demo_gif/blob/main/Word_cloud.gif)

### 7. Collections by style
&nbsp;
![7](https://github.com/lingzix/Demo_gif/blob/main/Collection.gif)

### 8. Portraits across time
&nbsp;
Loads 6 portraits initially, each from a century between 1400 - 2000. A shuffle button allows users to shuffle and load new portraits from each century. The purpose is for users to get a glimpse of the historical evolution of portrait painting styles over time.

![8](https://github.com/lingzix/Demo_gif/blob/main/Portraits.gif)

### 9. Distribution by type
&nbsp;
Users can select a term type from the menu (eg. style/school/theme/technique/keyword/place), and the chart will return the most common terms within that type.

![9](https://github.com/lingzix/Demo_gif/blob/main/Bar_chart.gif)


## Local Setup
If you would like a copy of the project source code, please contact me (Iris) via irismaxj@gmail.com .


1) Download the `WebApp_Gallery` folder to your local machine (ex. Mac, Win, Linux)

2) In your machine's CLI, `cd` to the `WebApp_Gallery` folder and use the following commands to start the web-application

| Command     | Description |
| -------     | ----------  |
| `npm install` | If first time running, `cd` to the `server` and `client` directories, install the dependencies for these two ends respectively.<br /> For subsequent launching on the same machine, no need to reinstall these dependencies.|
| `npm start` | First start running the `server` application , then launch the `client` application<br />Home-page should automatically be loaded and opened in a new broswer window (otherwise, go to this URL `http://localhost:3000/home` in your browser) |



## Additional Details 
### 1. Data Cleaning
Inside `DataCleaning` Directory, we kept in record of the processing of Raw Source Data into Cleaned Data, which are ready for MySQL DB population. The data source files are in `CSV` formate, and the data cleaning is performed with the help of `Python Pandas Library` inside `Jupyter Notebook` environment.  
All the cleaned up data source files are placed inside `Ready` subdirectory, and are used for initial database population.


### 2. Database Construction and Management
Inside `DatabaseManage` Directory, we kept in record of all the `MySQL` scripts that were used for populating database, managing database, and optimizing database.

### 3. Documentations
Refer to files inside `Documentations` for detailed documentations about this web-application's design, architectures, APIs, performance evaluations etc.
