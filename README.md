# Ex.08 Design of Interactive Image Gallery
## Date:18-12-2025
25019206
## AIM:
To design a web application for an inteactive image gallery with minimum five images.

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

## PROGRAM :
````
gallery.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Image Gallery</title>
    <link rel="stylesheet" href="gallery.css">
</head>
<body>

<div class="gallery-container">

    <div class="card">
        <img src="eren.jpg" alt="Eren">
    </div>

    <div class="card">
        <img src="guts.jpg" alt="Guts">
    </div>

    <div class="card main">
        <img src="throffin.jpg" alt="Thorffinn">
    </div>

    <div class="card">
        <img src="lelouch.jpg" alt="Lelouch">
    </div>

    <div class="card">
        <img src="miyamoto.jpg" alt="Miyamoto">
    </div>

</div>

<script src="gallery.js"></script>
</body>
</html>

gallery.css
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
}

body{
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(90deg, #0500ff, #00aaff);
    overflow: hidden;
}

/* Main gallery row */
.gallery-container{
    display: flex;
    align-items: center;
    gap: 70px;
}

/* Normal cards */
.card{
    width: 160px;
    height: 230px;
    border: 6px solid rgba(255,255,255,0.35);
    display: flex;
    justify-content: center;
    align-items: center;
    background: rgba(255,255,255,0.05);
    transition: all 0.4s ease;
    cursor: pointer;
}

/* Images */
.card img{
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Center focused card */
.card.main{
    width: 340px;
    height: 460px;
    border: 10px solid rgba(255,255,255,0.45);
    transform: scale(1.05);
}

/* Hover effect (small zoom only) */
.card:not(.main):hover{
    transform: scale(1.08);
}

/* Mobile view */
@media (max-width: 900px){
    .gallery-container{
        gap: 25px;
    }

    .card.main{
        width: 260px;
        height: 360px;
    }
}

gallery.js
const cards = document.querySelectorAll(".card");

cards.forEach(card => {
    card.addEventListener("click", () => {

        // remove main from all
        cards.forEach(c => c.classList.remove("main"));

        // add main to clicked
        card.classList.add("main");
    });
});


````

## OUTPUT:
<img width="1914" height="969" alt="igallery img" src="https://github.com/user-attachments/assets/620acda4-3300-42fb-8e30-e1ef830c83a1" />



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
