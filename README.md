# Ex.07 Design of Interactive Image Gallery
## Date: 23.12.2025

## AIM:
To design a web application for an inteactive image gallery for a minimum five images with next and previous buttons.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM:
```
gallery.html

<html>
<head>
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1> Image Gallery</h1>

    <div class="gallery-container">
        <img id="galleryImage" src="furniture.png" alt="Gallery Image">

        <div class="buttons">
            <button id="prevbutton">Previous</button>
            <button id="nextbutton">Next</button>
        </div>
    </div>


    <footer>
        <p>Designed & Developed by Saigokul.k © 2025</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

style.css

<html>
<head>
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1> Image Gallery</h1>

    <div class="gallery-container">
        <img id="galleryImage" src="furniture.png" alt="Gallery Image">

        <div class="buttons">
            <button id="prevbutton">Previous</button>
            <button id="nextbutton">Next</button>
        </div>
    </div>


    <footer>
        <p>Designed & Developed by Saigokul.k © 2025</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

script.js

const images = [
    "robot.png",
    "nature.png",
    "space.png"
    
];

let currentIndex = 0;

const galleryImage = document.getElementById("galleryImage");
const nextBtn = document.getElementById("nextbutton");
const prevBtn = document.getElementById("prevbutton");

nextBtn.addEventListener("click", () => {
    currentIndex = (currentIndex + 1) % images.length;
    galleryImage.src = images[currentIndex];
});

prevBtn.addEventListener("click", () => {
    currentIndex = (currentIndex - 1 + images.length) % images.length;
    galleryImage.src = images[currentIndex];
});

```

## OUTPUT:
![alt text](<Screenshot (42).png>) 
![alt text](<Screenshot (39).png>) 
![alt text](<Screenshot (40).png>) 
![alt text](<Screenshot (41).png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
