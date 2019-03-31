# feed.me
A solution for the millions of busy people worldwide struggling to incorporate cooking into their daily lives, developed at NewHacks by [Ahmad](https://github.com/ahmadtc1), [JY](https://github.com/grandpabear), [Max](https://github.com/Maxeraph), and Grace.

This solution placed second in the sustainibility category at the University of Toronto's NewHacks hackathon


## Usage
feed.me is as easy as 1, 2, 3...

Through feed.me's simple and easy to use user interface, users can snap a picture of their receipt on their phone, and then submit it. Once their picture is submitted, our backend logic takes care of using OCR to digitize the text and upload the ingredients to our server's database, where the ingredients are then used to return appropriate recipes to our users right back on their phone


## Technical Details

#### Front-End
Our app's user interface was designed using Android Studio by our App developers, [JY](https://github.com/grandpabear), and Grace.

#### Server Side Logic
[I](https://github.com/ahmadtc1) developed a web server through which the requests between the Android App and database were processed. The server was developed using Python's Flask framework, where I developed a REST Api, accessible at different endpoints for reading and writing data. My database of choice was MongoDB, as I love its flexibility and storage formats. I utilised POST requests to insert data into the database, and GET requests to retrieve data from the database.


#### Computer Vision
The computer vision was handled by [Max](https://github.com/Maxeraph), who used the Google Cloud Vision API to recognize receipt text and trained a model to localize objects if scanning the ingredients in the fridge rather than the receipt.


#### UI
![Home Page](/Images/55539239_425496811591103_5437915074796716032_n.png)

![Recipes](/Images/54522371_865201980485925_2345966563628154880_n.png)
