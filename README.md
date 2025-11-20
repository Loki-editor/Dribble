# Project Responsive Web Design using Bootstrap
## Date: 20-11-2025

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
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Keralam Tourism – Simplified</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" />
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-light bg-light border-bottom sticky-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#">Keralam Tourism</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navTN">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navTN">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link active" href="#home">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#destinations">Destinations</a></li>
          <li class="nav-item"><a class="nav-link" href="#plan">Plan</a></li>
          <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Carousel -->
  <header id="home" class="bg-light">
    <div id="tnCarousel" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-indicators">
        <button type="button" data-bs-target="#tnCarousel" data-bs-slide-to="0" class="active"></button>
        <button type="button" data-bs-target="#tnCarousel" data-bs-slide-to="1"></button>
        <button type="button" data-bs-target="#tnCarousel" data-bs-slide-to="2"></button>
      </div>

      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="kerala_backwaters.png" class="d-block w-100"alt="Kerala Backwaters">
          <div class="carousel-caption d-none d-md-block">
            <h5 class="fw-bold">Alleppey Backwaters</h5>
            <p>Tranquil houseboats and coconut-fringed waterways.</p>
          </div>
        </div>

        <div class="carousel-item">
          <img src="munnar.png" class="d-block w-100" alt="Munnar Hills">
          <div class="carousel-caption d-none d-md-block">
            <h5 class="fw-bold">Munnar Hills</h5>
            <p>Rolling tea estates and misty green mountain ranges.</p>
          </div>
        </div>

        <div class="carousel-item">
          <img src="kovalam.png" class="d-block w-100" alt="Kovalam Beach">
          <div class="carousel-caption d-none d-md-block">
            <h5 class="fw-bold">Kovalam Beach</h5>
            <p>Golden shores and iconic lighthouse views.</p>
          </div>
        </div>
      </div>

      <button class="carousel-control-prev" type="button" data-bs-target="#tnCarousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#tnCarousel" data-bs-slide="next">
        <span class="carousel-control-next-icon"></span>
      </button>
    </div>
  </header>

  <section class="py-5">
    <div class="container text-center">
      <h1 class="display-6 fw-bold">Discover Keralam</h1>
      <p class="lead text-muted mb-0">
        Known as “God’s Own Country”, Kerala offers backwaters, beaches, wildlife, Ayurvedic resorts, and lush hill stations.
      </p>
    </div>
  </section>

  <!-- Destinations -->
  <section id="destinations" class="py-5 bg-light">
    <div class="container">
      <div class="d-flex align-items-center justify-content-between mb-4">
        <h2 class="h3 m-0">Top Destinations</h2>
        <div class="btn-group">
          <a class="btn btn-outline-secondary active" href="#destinations">All</a>
          <a class="btn btn-outline-secondary" href="#plan">Plan</a>
        </div>
      </div>

      <div class="row g-4">
        
        <!-- Alleppey -->
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card border-0 shadow-sm h-100">
            <img src="alleppey.png" class="card-img-top" alt="Alleppey Backwaters">
            <div class="card-body">
              <h5 class="card-title">Alleppey</h5>
              <p class="card-text text-muted">Famous for houseboats, serene canals, and village life.</p>
              <a href="#contact" class="btn btn-dark btn-sm">Ask for details</a>
            </div>
          </div>
        </div>

        <!-- Munnar -->
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card border-0 shadow-sm h-100">
            <img src="munnar.png" class="card-img-top" alt="Munnar">
            <div class="card-body">
              <h5 class="card-title">Munnar</h5>
              <p class="card-text text-muted">Tea plantations, waterfalls, and cool climate.</p>
              <a href="#contact" class="btn btn-dark btn-sm">Ask for details</a>
            </div>
          </div>
        </div>

        <!-- Kochi -->
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card border-0 shadow-sm h-100">
            <img src="kochi.png" class="card-img-top" alt="Kochi">
            <div class="card-body">
              <h5 class="card-title">Kochi</h5>
              <p class="card-text text-muted">Chinese fishing nets, heritage streets, and coastal beauty.</p>
              <a href="#contact" class="btn btn-dark btn-sm">Ask for details</a>
            </div>
          </div>
        </div>

        <!-- Wayanad -->
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card border-0 shadow-sm h-100">
            <img src="wayanad.png" class="card-img-top" alt="Wayanad">
            <div class="card-body">
              <h5 class="card-title">Wayanad</h5>
              <p class="card-text text-muted">Wildlife sanctuaries, caves, and lush greenery.</p>
              <a href="#contact" class="btn btn-dark btn-sm">Ask for details</a>
            </div>
          </div>
        </div>

        <!-- Kovalam -->
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card border-0 shadow-sm h-100">
            <img src="kovalam.png" class="card-img-top" alt="Kovalam Beach">
            <div class="card-body">
              <h5 class="card-title">Kovalam</h5>
              <p class="card-text text-muted">Popular beach destination with a lighthouse view.</p>
              <a href="#contact" class="btn btn-dark btn-sm">Ask for details</a>
            </div>
          </div>
        </div>

        <!-- Thekkady -->
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card border-0 shadow-sm h-100">
            <img src="thekkady.png" class="card-img-top" alt="Thekkady">
            <div class="card-body">
              <h5 class="card-title">Thekkady</h5>
              <p class="card-text text-muted">Periyar Wildlife Sanctuary and boat safari.</p>
              <a href="#contact" class="btn btn-dark btn-sm">Ask for details</a>
            </div>
          </div>
        </div>
      </div>

      <div class="text-center mt-5">
        <a href="#plan" class="btn btn-outline-dark btn-lg">Plan Your Trip</a>
      </div>
    </div>
  </section>

  <!-- Plan Section -->
  <section id="plan" class="py-5">
    <div class="container">
      <h2 class="h3 text-center mb-4">Plan Your Visit</h2>
      <div class="accordion" id="planAccordion">

        <div class="accordion-item">
          <h2 class="accordion-header">
            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne">
              Best Time To Visit
            </button>
          </h2>
          <div id="collapseOne" class="accordion-collapse collapse show">
            <div class="accordion-body">
              September to March is ideal for beaches, wildlife, and backwaters. Summers suit hill stations like Munnar and Wayanad.
            </div>
          </div>
        </div>

        <div class="accordion-item">
          <h2 class="accordion-header">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo">
              Getting Around
            </button>
          </h2>
          <div id="collapseTwo" class="accordion-collapse collapse">
            <div class="accordion-body">
              Buses and trains connect all major cities. Hire taxis for hill stations and wildlife routes.
            </div>
          </div>
        </div>

        <div class="accordion-item">
          <h2 class="accordion-header">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree">
              Local Food To Try
            </button>
          </h2>
          <div id="collapseThree" class="accordion-collapse collapse">
            <div class="accordion-body">
              Appam, Puttu, Kerala Sadhya, Fish Curry, Malabar Biryani, and Banana Chips.
            </div>
          </div>
        </div>
      </div>

      <!-- Stats -->
      <div class="row text-center mt-5">
        <div class="col-6 col-md-3">
          <h3 class="fw-bold">6+</h3>
          <p class="text-muted">Top Destinations</p>
        </div>
        <div class="col-6 col-md-3">
          <h3 class="fw-bold">44</h3>
          <p class="text-muted">Rivers</p>
        </div>
        <div class="col-6 col-md-3 mt-4 mt-md-0">
          <h3 class="fw-bold">2</h3>
          <p class="text-muted">Major Hill Stations</p>
        </div>
        <div class="col-6 col-md-3 mt-4 mt-md-0">
          <h3 class="fw-bold">1</h3>
          <p class="text-muted">Backwater State</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="py-5 bg-light">
    <div class="container">
      <div class="row g-4 align-items-center">
        <div class="col-lg-6">
          <h2 class="h3 mb-3">Contact</h2>
          <p class="text-muted">Planning a Kerala trip? Send your query—we'll help you build a perfect itinerary.</p>
          <ul class="list-unstyled">
            <li>📍 Thiruvananthapuram, Kerala</li>
            <li>📞 +91 98765 43210</li>
            <li>📧 travel@keralamtour.in</li>
          </ul>
        </div>

        <div class="col-lg-6">
          <form class="p-3 border rounded-3 bg-white">
            <div class="mb-3">
              <label class="form-label">Name</label>
              <input type="text" class="form-control" placeholder="Your name" />
            </div>
            <div class="mb-3">
              <label class="form-label">Email</label>
              <input type="email" class="form-control" placeholder="name@example.com" />
            </div>
            <div class="mb-3">
              <label class="form-label">Message</label>
              <textarea class="form-control" rows="3" placeholder="What would you like to know?"></textarea>
            </div>
            <button type="submit" class="btn btn-dark">Send</button>
          </form>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-dark text-white text-center py-4">
    <div class="container">
      <p class="mb-1">© 2025 Keralam Tourism</p>
      <p class="mb-0">Designed by <strong>LOKESH </strong></p>
    </div>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot (19).png>)

![alt text](<Screenshot (20).png>) 

![alt text](<Screenshot (21).png>) 

![alt text](<Screenshot (22).png>) 

![alt text](<Screenshot (23).png>) 

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
