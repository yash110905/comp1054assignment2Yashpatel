<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Album Layout with 3D Hover</title>
  <!-- Bootstrap 4.5.2  -->
  <!-- taken from "https://stackpath.bootstrapcdn.com" -->
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <link rel="stylesheet" href="style.css">
</head>

<body>
    <!-- option button with dropdown -->
<div class="option-menu">
  <button class="option-btn"> ☰ </button>
  <div class="dropdown-panel">
    <a href="#">About Us</a>
    <a href="#">Contact</a>
    <a href="#">Follow on Twitter</a>
    <a href="#">Like on Facebook</a>
  </div>
</div>
  <header style="background-color: #333; padding: 10px;">
  <div style="max-width: 960px; margin: 0 auto; display: flex; justify-content: space-between; align-items: center;">
    <a href="#" style="color: white; text-decoration: none; font-weight: bold; font-size: 1.2rem;">
      Album
    </a>
  </div>
</header>


  <!-- hero banner -->
  <section class="hero text-center bg-light mb-0">

    <div class="container">
      <h1 class="hero-heading">Album example</h1>
      <p class="lead text-muted">Something short and leading about the collection below—its contents, the creator, etc.</p>
      <p>
        <a href="#" class="btn btn-primary my-2">Primary Action</a>
        <a href="#" class="btn btn-secondary my-2">Secondary Action</a>
      </p>
    </div>
  </section>

  <!-- Album Grid -->
  <div class="album py-5 bg-light">
    <div class="container">
      <div class="row">
        <!-- multiple cards with random images -->
        <div class="col-md-4">
          <div class="card shadow-sm custom-card">
            <img src="https://html.phoenixcoded.net/light-able/bootstrap/assets/images/light-box/l3.jpg" class="card-img-top" alt="Image">
            <div class="card-body">
              <p class="card-text">This is a wider card with supporting text below as a natural lead-in.</p>
              <div class="d-flex justify-content-between align-items-center">
                <div class="btn-group">
                  <button class="btn btn-sm btn-outline-primary">View</button>
                  <button class="btn btn-sm btn-outline-secondary">Edit</button>
                </div>
                <small class="text-muted">9 mins</small>
              </div>
            </div>
          </div>
        </div>

        <!-- Duplicate with different images -->
        <div class="col-md-4"><div class="card shadow-sm custom-card"><img src="https://images.pexels.com/photos/459225/pexels-photo-459225.jpeg?cs=srgb&dl=daylight-environment-forest-459225.jpg&fm=jpg" class="card-img-top"><div class="card-body"><p class="card-text">Another beautiful photo for this album collection.</p><div class="d-flex justify-content-between align-items-center"><div class="btn-group"><button class="btn btn-sm btn-outline-primary">View</button><button class="btn btn-sm btn-outline-secondary">Edit</button></div><small class="text-muted">12 mins</small></div></div></div></div>
        <div class="col-md-4"><div class="card shadow-sm custom-card"><img src="https://images.pexels.com/photos/236047/pexels-photo-236047.jpeg?cs=srgb&dl=clouds-cloudy-countryside-236047.jpg&fm=jpg" class="card-img-top"><div class="card-body"><p class="card-text">Cool shot to enhance the gallery aesthetics.</p><div class="d-flex justify-content-between align-items-center"><div class="btn-group"><button class="btn btn-sm btn-outline-primary">View</button><button class="btn btn-sm btn-outline-secondary">Edit</button></div><small class="text-muted">15 mins</small></div></div></div></div>
        <div class="col-md-4"><div class="card shadow-sm custom-card"><img src="https://tse4.mm.bing.net/th/id/OIP.PikUdeXdPP5f3FAwKZYtlQHaJQ?r=0&rs=1&pid=ImgDetMain&o=7&rm=3" class="card-img-top"><div class="card-body"><p class="card-text">Supporting text that naturally flows into additional content.</p><div class="d-flex justify-content-between align-items-center"><div class="btn-group"><button class="btn btn-sm btn-outline-primary">View</button><button class="btn btn-sm btn-outline-secondary">Edit</button></div><small class="text-muted">18 mins</small></div></div></div></div>
        <div class="col-md-4"><div class="card shadow-sm custom-card"><img src="https://cdn.pixabay.com/photo/2020/10/23/07/18/sea-5677914_640.jpg" class="card-img-top"><div class="card-body"><p class="card-text">Another sample card with a beautiful thumbnail.</p><div class="d-flex justify-content-between align-items-center"><div class="btn-group"><button class="btn btn-sm btn-outline-primary">View</button><button class="btn btn-sm btn-outline-secondary">Edit</button></div><small class="text-muted">21 mins</small></div></div></div></div>
        <div class="col-md-4"><div class="card shadow-sm custom-card"><img src="https://i.pinimg.com/originals/27/bc/87/27bc8773c7f33522a73989315866eb66.jpg" class="card-img-top"><div class="card-body"><p class="card-text">Clean and simple design to match the album layout.</p><div class="d-flex justify-content-between align-items-center"><div class="btn-group"><button class="btn btn-sm btn-outline-primary">View</button><button class="btn btn-sm btn-outline-secondary">Edit</button></div><small class="text-muted">30 mins</small></div></div></div></div>
      </div>
    </div>
  </div>
  <!-- footer -->
  <footer class="text-muted text-center py-4 bg-dark text-white">
    <div class="container">
      <p class="mb-1">Assignment 2 css @2025</p>
    </div>
  </footer>
  <script>
document.addEventListener("DOMContentLoaded", function () {
  const optionBtn = document.querySelector(".option-btn");
  const dropdown = document.querySelector(".dropdown-panel");

  optionBtn.addEventListener("click", function () {
    dropdown.classList.toggle("show");
  });
});
</script>

</body>
</html>

/* general styles */
body {
  background: #f8f9fa;
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

/* navbar */
.navbar {
  background: #343a40;
}

/* hero section */
.hero {
  margin-bottom: 0;
  
}


/* footer */
footer {
  background: #343a40;
  color: white;
}
footer p {
  margin: 0;
}

/*album grid */
.album {
  padding: 40px 0;
}
.row > div {
  margin-bottom: 30px; 
}

/*  custom cards  */
.custom-card {
  height: 100%;
  display: flex;
  flex-direction: column;
  border-radius: 8px;
  overflow: hidden;
  transition: transform 0.4s ease, box-shadow 0.4s ease;
}

.custom-card img {
  height: 200px;
  object-fit: cover;
}

/* card body padding & layout */
.custom-card .card-body {
  flex: 1;
  padding: 1.25rem;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

/* 3D hover effect */
.custom-card:hover {
  transform: scale(1.05) rotateY(4deg);
  box-shadow: 0 12px 25px rgba(0, 0, 0, 0.25);
}

/* top-right option button  */
.option-menu {
  position: fixed;
  top: 15px;
  right: 20px;
  z-index: 1000;
}

/* button styling */
.option-btn {
  width: 45px;
  height: 40px;
  background: #343a40;
  border: 2px solid #fff;
  border-radius: 6px;
  color: white;
  font-size: 24px;
  cursor: pointer;
  transition: background 0.3s, transform 0.2s;
}

.option-btn:hover {
  background: #495057;
  transform: scale(1.05);
}

/* dropdown menu */
.dropdown-panel {
  display: none;
  flex-direction: column;
  position: absolute;
  top: 50px;
  right: 0;
  background: #212529;
  border: 1px solid #444;
  border-radius: 6px;
  min-width: 180px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.3);
}

/* Dropdown links */
.dropdown-panel a {
  padding: 10px;
  color: #fff;
  text-decoration: none;
  display: block;
  border-bottom: 1px solid #444;
  transition: background 0.3s;
}

.dropdown-panel a:last-child {
  border-bottom: none;
}

.dropdown-panel a:hover {
  background: #495057;
}

/* Show dropdown when toggled */
.dropdown-panel.show {
  display: flex;
}
