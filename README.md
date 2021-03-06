# Mission to Mars

Flask web application that scrapes various websites for data related to the Mars Mission and displays the information in a single HTML page.

#### Scrapping

##### NASA Mars News
  * Script collects the latest News Title and Paragraph Text.

##### JPL Mars Space Images - Featured Image

  * Script finds the image url for the current Featured Mars Image and assigns the url string of the full size image.

##### Mars Weather

   * Script visits the Mars Weather twitter account and scrapes the latest Mars weather tweet.

##### Mars Facts

   * Script visit the Mars Facts webpage and uses Pandas to scrape the table containing facts about the planet including Diameter, Mass, etc.

##### Mars Hemispheres

   * Script visits the USGS Astrogeology site and obtains the full resolution images for each of Mars' hemispheres.

#### MongoDB and Flask Application

The MongoDB is currently hosted on the Database-as-a-Service https://mlab.com/. It requires a config.py file (hidden) using a driver via the standard MongoDB URI. The config.py contains a variable "authentication=" set to the MongoDB URI.

![Test Image 3](https://github.com/mserobabina/web-scraping-challenge/blob/master/Missions_to_Mars/Capture.PNG)
 
Alternatively, it can run locally. First, install MongoDB. Once MongoDB is installed run the command mondgod on bash. Don't forget to comment and uncomment the URI to use the local database only. Also comment out `import config`.

#### Requirements
 ##### Modules Required
       * pandas==0.23.3
       * splinter==0.9.0
       * pymongo==3.7.1
       * numpy==1.15.0
       * Flask==1.0.2
       * requests==2.18.4
       * beautifulsoup4==4.6.3
       * gunicorn==19.9.0
       * lxml==4.2.5
       * Jinja2==2.10
       * beautifulsoup4==4.6.3
       * bs4==0.0.1
       * Flask-PyMongo==2.1.0
 ![Test Image 4](https://github.com/mserobabina/web-scraping-challenge/blob/master/Missions_to_Mars/screenshot_mars.png)
 
