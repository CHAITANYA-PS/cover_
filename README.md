# Ex.06 Book Front Cover Page Design
## Date: 05.11.25

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fundamentals of Web Application Development</title>

  <style>
    body {
      background: radial-gradient(circle at center, #0a0a0a 40%, #1b1b1b);
      color: #fff;
      font-family: 'Georgia', serif;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }

    .book-cover {
      position: relative;
      background-image: url('file:///C:/Users/chait/Downloads/WEB/cover_/chaitu/static/images/bg.png');
      background-size: cover;
      background-position: center;
      border: 2px solid #aa0000;
      border-radius: 12px;
      padding: 40px 60px;
      width: 420px;
      text-align: center;
      box-shadow: 0 0 40px rgba(255, 0, 0, 0.5);
      overflow: hidden;
    }
    .book-cover::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.5);
      border-radius: 12px;
      z-index: 0;
    }

    .book-cover * {
      position: relative;
      z-index: 1;
    }

    .top-section {
      text-align: left;
      color: #ff5555;
      font-weight: bold;
      border-bottom: 1px solid #ff5555;
      padding-bottom: 6px;
      margin-bottom: 20px;
    }

    .title-section h1 {
      color: #ff2e2e;
      font-size: 28px;
      line-height: 1.3;
      letter-spacing: 1px;
      text-shadow: 0 0 10px rgba(255, 0, 0, 0.6);
    }

    .subtitle {
      color: #f8bcbc;
      margin: 10px 0 20px 0;
      font-size: 14px;
    }

    .image-section {
      margin: 25px 0;
    }

    .book-image {
      width: 220px;
      height: 300px;
      object-fit: cover;
      border-radius: 8px;
      box-shadow: 0 0 20px rgba(255, 0, 0, 0.4);
    }

    .edition {
      color: #00aaff;
      font-weight: bold;
      font-size: 16px;
      text-decoration: underline;
      margin: 10px 0;
    }

    .bottom-section {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-top: 25px;
      font-weight: bold;
    }

    .author {
      color: #ff4444;
    }

    .publisher-end {
      color: #ff4444;
    }

    .author-photo {
      position: absolute;
      bottom: 15px;
      right: 15px;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      object-fit: cover;
      border: 2px solid #f80000;
      box-shadow: 0 0 10px rgba(157, 71, 71, 0.5);
      z-index: 2;
    }
    .book-cover {
      opacity: 0;
      transform: translateY(20px);
      animation: fadeInUp 1s ease forwards;
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
</head>
<body>
  <div class="book-cover">
    <div class="top-section">
      <h3 class="publisher">GOT
      </h3>
    </div>

    <div class="title-section">
        <h1>The Song of Ice And Fire</h1>
      <p class="subtitle">The seven kingdoms are the North, the Vale, the Iron Islands, the Westerlands, the Stormlands, the Reach, and Dorne.</p>
    </div>

    <div class="image-section">
      <img src="file:///C:/Users/chait/Downloads/WEB/cover_/chaitu/static/images/in.png" alt="Game of Thrones Theme" class="book-image">
    </div>

    <div class="bottom-section">
      <span class="author">George RR Martin</span>
    </div>

    <img src="file:///C:/Users/chait/Downloads/WEB/cover_/chaitu/static/images/au.png" alt="Author Photo" class="author-photo">
  </div>
</body>
</html>

```

## OUTPUT:
<img width="1915" height="1033" alt="image" src="https://github.com/user-attachments/assets/acab9741-172a-4973-b392-295e9843c58a" />


## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
