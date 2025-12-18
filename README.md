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
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Image Gallery</title>
  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    body{
      min-height:100vh;
      display:flex;
      justify-content:center;
      align-items:center;
      background: linear-gradient(90deg, #0a00ff, #00b4ff);
    }

    .gallery{
      width:100%;
      display:flex;
      justify-content:center;
      align-items:center;
      gap:80px;
    }

    .card{
      width:160px;
      height:220px;
      border:6px solid rgba(255,255,255,0.25);
      display:flex;
      justify-content:center;
      align-items:center;
      background: transparent;
    }

    .card img{
      width:100%;
      height:100%;
      object-fit:cover;
    }

    /* Center main image */
    .card.main{
      width:320px;
      height:420px;
      border:10px solid rgba(255,255,255,0.35);
    }

    @media(max-width:900px){
      .gallery{
        gap:30px;
      }
      .card.main{
        width:260px;
        height:360px;
      }
    }
  </style>
</head>
<body>

  <div class="gallery">

    <div class="card">
      <img src="eren.jpg" alt="character 1">
    </div>

    <div class="card">
      <img src="miyamoto.jpg" alt="character 2">
    </div>

    <div class="card main">
      <img src="guts.jpg" alt="peace character">
    </div>

    <div class="card">
      <img src="lelouch.jpg" alt="character 4">
    </div>

    <div class="card">
      <img src="throffin.jpg" alt="character 5">
    </div>

  </div>

</body>
</html>
````

## OUTPUT:
<img width="1920" height="1080" alt="igallery" src="https://github.com/user-attachments/assets/7dfa31d8-7a0b-4b08-ae3f-cca9c8a5eeca" />



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
