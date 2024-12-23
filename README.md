# Project Responsive Web Design using Bootstrap
## Date:23/12/2024

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
dri.html
<STYLE>
body {
    background: linear-gradient(lightblue, teal);
  }
  .navbar {
    background-color: #08C2FF;
  }
  .navbar .nav-link {
    color: white;
    font-weight: bold;
    margin: 0 10px;
  }
  .navbar .nav-link:hover {
    color: #16a085;
  }
  .sorting-navbar {
    background-color: #006BFF;
    color: white;
    padding: 10px 0;
  }
  .sorting-navbar .nav-link {
    color: white;
    font-weight: bold;
    margin: 0 10px;
    border: 2px solid transparent;
    border-radius: 5px;
    padding: 5px 15px;
  }
  .sorting-navbar .nav-link:hover {
    background-color: #2c3e50;
    border-color: white;
  }
  .card {
    border: none;
    border-radius: 15px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s, box-shadow 0.3s;
  }
  .card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
  }
  .card img {
    height: 150px;
    /* width: 150px; */
    background-size: cover;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
  }
  .card-body {
    background-color: #006BFF;
    color: white;
    text-align: center;
  }
  footer {
    margin-top: 50px;
    background-color: #08C2FF;
    color: white;
  }
  
  .about-section {
    background-color: #ecf0f1;
    padding: 50px 20px;
  }
  .about-section h2 {
    font-size: 2.5rem;
    font-weight: bold;
    color: #2c3e50;
  }
  
  /* Services Section */
  .services-section {
    background-color: #1abc9c;
    color: white;
    padding: 50px 20px;
  }
  .services-section h2 {
    font-size: 2.5rem;
    font-weight: bold;
  }
  .service-card {
    border: none;
    border-radius: 10px;
    background-color: white;
    color: #2c3e50;
    text-align: center;
    padding: 20px;
    transition: transform 0.3s, box-shadow 0.3s;
  }
  .service-card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  }
</STYLE>
  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dribble</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <nav class="navbar navbar-expand-lg">
    <div class="container">
      <a class="navbar-brand text-white" href="#">Dribble</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="about.html">About</a></li>
          <li class="nav-item"><a class="nav-link" href="service.html">Services</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <nav class="sorting-navbar">
    <div class="container d-flex justify-content-center">
      <ul class="nav">
        <li class="nav-item">
          <a class="nav-link active" href="#">Popular</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Newest</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Random</a>
        </li>
      </ul>
    </div>
  </nav>

  <div class="container my-5">
    <div class="row g-4">
      <div class="col-6 col-md-3">
        <div class="card">
          <img src="ai-generated-beautiful-nature-mountain-scenery-professionalgraphy-photo.jpg" class="card-img-top" alt="Placeholder">
          <div class="card-body">
            <h6 class="card-title">Card 1</h6>
          </div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="card">
          <img src="beautiful-nature-pictures-syv21loi30wdz7i2.jpg" class="card-img-top" alt="Placeholder">
          <div class="card-body">
            <h6 class="card-title">Card 2</h6>
          </div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="card">
          <img src="beautiful-nature-scenery-wallpaper-view_1123191-729.avif" class="card-img-top" alt="Placeholder">
          <div class="card-body">
            <h6 class="card-title">Card 3</h6>
          </div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="card">
          <img src="erawan-waterfall-thailand-beautiful-nature-background-42008912.webp" class="card-img-top" alt="Placeholder">
          <div class="card-body">
            <h6 class="card-title">Card 4</h6>
          </div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="card">
          <img src="europe-croatia-plitvice-lakes-main-waterfalls-spring-small.jpg" class="card-img-top" alt="Placeholder">
          <div class="card-body">
            <h6 class="card-title">Card 5</h6>
          </div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="card">
          <img src="landscape-sky-full-moon-seascape-to-night-serenity-nature-beautiful-view-sea-many-stars-attractive-dark-cloud-141554532.webp" class="card-img-top" alt="Placeholder">
          <div class="card-body">
            <h6 class="card-title">Card 6</h6>
          </div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="card">
          <img src="pexels-pixabay-206359.jpg" class="card-img-top" alt="Placeholder">
          <div class="card-body">
            <h6 class="card-title">Card 7</h6>
          </div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="card">
          <img src="scenic-view-waterfall-rocks-autumn_1048944-14210465.avif" class="card-img-top" alt="Placeholder">
          <div class="card-body">
            <h6 class="card-title">Card 8</h6>
          </div>
        </div>
      </div>
    </div>
  </div>

  <section id="contact" class="contact-section">
    <div class="container">
      <h2>Contact Us</h2>
      <form>
        <div class="mb-3">
          <label for="name" class="form-label">YOUR NAME</label>
          <input type="text" class="form-control" id="name" placeholder="Enter your name">
        </div>
        <div class="mb-3">
          <label for="email" class="form-label">YOUR EMAIL</label>
          <input type="email" class="form-control" id="email" placeholder="Enter your email">
        </div>
        <div class="mb-3">
          <label for="message" class="form-label">Message</label>
          <textarea class="form-control" id="message" rows="3" placeholder="Your message"></textarea>
        </div>
        <button type="submit" class="btn btn-primary">Send</button>
      </form>
    </div>
  </section>

  <footer class="text-center py-3">
    <p>&copy; 2024 Dribble. All rights reserved.</p>
  </footer>
</body>
</html>
home.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nature's Beauty</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: #333;
        }
        header {
            background-image: url('https://example.com/nature-banner.jpg'); 
            background-size: cover;
            background-position: center;
            color: white;
            padding: 50px 20px;
            text-align: center;
        }
        header h1 {
            font-size: 3em;
            margin: 0;
        }
        header p {
            font-size: 1.5em;
            margin: 10px 0 0;
        }
        nav {
            background-color: #4CAF50;
            color: white;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        section {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        section h2 {
            font-size: 2em;
            margin-bottom: 10px;
        }
        section p {
            line-height: 1.6;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Nature's Beauty</h1>
        <p>Explore the wonders of the natural world</p>
    </header>
    <nav>
        <a href="#about">About</a>
        <a href="#gallery">Gallery</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="about">
        <h2>About Nature</h2>
        <p>Nature is the most beautiful and precious gift of God to humans. It includes everything we see around us, from the majestic mountains to the serene rivers, lush green forests, and vibrant wildlife. Our mission is to inspire people to appreciate and protect the natural world.</p>
    </section>
    <section id="gallery">
        <h2>Gallery</h2>
        <p>Here are some breathtaking snapshots of nature:</p>
       
        <img src="ai-generated-beautiful-nature-mountain-scenery-professionalgraphy-photo.jpg" alt="Nature Image 1" style="width:100%;max-width:600px;">
        <img src="beautiful-nature-pictures-syv21loi30wdz7i2.jpg" alt="Nature Image 2" style="width:100%;max-width:600px;">
    </section>
    <section id="contact">
        <h2>Contact Us</h2>
        <p>Have questions or want to share your nature experiences? Reach out to us!</p>
        <p>Email: thiru@gmail.com</p>
    </section>
    <footer>
        <p>&copy; 2024 Nature's Beauty. All rights reserved.</p>
    </footer>
</body>
</html>

service .html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Our Services</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f9fa;
            color: #333;
        }
        header {
            background-color: #007BFF;
            color: white;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            font-size: 2.5em;
            margin: 0;
        }
        section {
            padding: 20px;
            max-width: 800px;
            margin: 20px auto;
            background: #ffffff;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        section h2 {
            font-size: 2em;
            margin-bottom: 10px;
            color: #007BFF;
        }
        section p {
            line-height: 1.6;
            margin: 10px 0;
        }
        ul {
            list-style-type: disc;
            padding-left: 20px;
        }
        ul li {
            margin: 10px 0;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Our Services</h1>
    </header>
    <section>
        <h2>What We Offer</h2>
        <p>We provide a variety of services to help you connect with and preserve the natural world. Our mission is to make nature accessible, enjoyable, and sustainable for everyone.</p>
        <ul>
            <li><strong>Nature Tours:</strong> Guided tours through breathtaking natural landscapes.</li>
            <li><strong>Wildlife Conservation:</strong> Programs to protect and preserve endangered species.</li>
            <li><strong>Eco-Friendly Workshops:</strong> Learn how to live sustainably and reduce your carbon footprint.</li>
            <li><strong>Community Cleanups:</strong> Join us in making our environment cleaner and greener.</li>
            <li><strong>Educational Seminars:</strong> Inspiring talks and sessions on the importance of nature conservation.</li>
        </ul>
    </section>
    <footer>
        <p>&copy; 2024 Our Services. All rights reserved.</p>
    </footer>
</body>
</html>
about.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Nature</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #eaf7f0;
            color: #333;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            font-size: 2.5em;
            margin: 0;
        }
        section {
            padding: 20px;
            max-width: 800px;
            margin: 20px auto;
            background: #ffffff;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        section h2 {
            font-size: 2em;
            margin-bottom: 10px;
            color: #4CAF50;
        }
        section p {
            line-height: 1.6;
            margin: 10px 0;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>About Nature</h1>
    </header>
    <section>
        <h2>Our Connection to Nature</h2>
        <p>Nature is a vast and beautiful phenomenon that encompasses all living and non-living things on Earth. From the towering mountains and deep oceans to the smallest insects and microorganisms, nature's diversity is endless and awe-inspiring.</p>
        <p>Understanding and appreciating nature is essential for the survival of all species, including humans. It provides us with essential resources like air, water, and food, as well as inspiration and solace.</p>
    </section>
    <section>
        <h2>Why Protect Nature?</h2>
        <p>Protecting nature is crucial to maintaining the balance of ecosystems. Every species, no matter how small, plays a role in this balance. Deforestation, pollution, and climate change pose serious threats to the natural world, making conservation efforts more important than ever.</p>
        <p>By adopting sustainable practices and supporting conservation initiatives, we can ensure that future generations experience the beauty and benefits of nature.</p>
    </section>
    <footer>
        <p>&copy; 2024 About Nature. All rights reserved.</p>
    </footer>
</body>
</html>
contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f9fa;
            color: #333;
        }
        header {
            background-color: #28a745;
            color: white;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            font-size: 2.5em;
            margin: 0;
        }
        section {
            padding: 20px;
            max-width: 800px;
            margin: 20px auto;
            background: #ffffff;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        section h2 {
            font-size: 2em;
            margin-bottom: 10px;
            color: #28a745;
        }
        section p {
            line-height: 1.6;
            margin: 10px 0;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        form label {
            margin: 10px 0 5px;
            font-weight: bold;
        }
        form input, form textarea, form button {
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 1em;
        }
        form button {
            background-color: #28a745;
            color: white;
            border: none;
            cursor: pointer;
        }
        form button:hover {
            background-color: #218838;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Contact Us</h1>
    </header>
    <section>
        <h2>Get in Touch</h2>
        <p>If you have any questions, feedback, or just want to say hello, feel free to reach out to us using the form below. We'd love to hear from you!</p>
        <form>
            <label for="name">Name</label>
            <input type="text" id="name" name="name" placeholder="Your Name" required>

            <label for="email">Email</label>
            <input type="email" id="email" name="email" placeholder="Your Email" required>

            <label for="message">Message</label>
            <textarea id="message" name="message" rows="5" placeholder="Your Message" required></textarea>

            <button type="submit">Send Message</button>
        </form>
    </section>
    <footer>
        <p>&copy; 2024 Contact Us. All rights reserved.</p>
    </footer>
</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2024-12-23 110211.png>)
![alt text](<Screenshot 2024-12-23 110225.png>)
![alt text](<Screenshot 2024-12-23 110241.png>)
![alt text](<Screenshot 2024-12-23 110251.png>)
![alt text](<Screenshot 2024-12-23 110304.png>)
![alt text](<Screenshot 2024-12-23 110317.png>)
![alt text](<Screenshot 2024-12-23 110330.png>)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
