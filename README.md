<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Banner with Large Nav Gap</title>
<style>
  body {
    margin: 0;
    background-color: #fbfbf9;
    font-family: Arial, sans-serif;
  }
  .banner-container {
    position: relative;
    width: 100%;
    max-height: 300px;
  }
  .banner {
    width: 100%;
    max-height: 300px;
    object-fit: cover;
    display: block;
  }
  nav.navbar {
    position: absolute;
    top: 0;
    width: 100%;
    display: flex;
    justify-content: center;
    gap: 200px; /* BIGGER gap between nav groups */
    background-color: rgba(251, 251, 249, 0.7);
    padding: 15px 30px;
    box-sizing: border-box;
    backdrop-filter: saturate(180%) blur(10px);
    z-index: 10;
  }
  .nav-group {
    display: flex;
    gap: 30px;
  }
  .nav-link {
    font-size: 18px;
    color: black;
    text-decoration: none;
    font-weight: 600;
  }
  .nav-link:hover {
    text-decoration: underline;
  }
</style>
</head>
<body>

<div class="banner-container">
  <nav class="navbar" role="navigation" aria-label="Primary navigation">
    <div class="nav-group">
      <a href="our-team.html" class="nav-link">Our Team</a>
      <a href="publications.html" class="nav-link">Publications</a>
      <a href="projects.html" class="nav-link">Projects</a>
    </div>
    <div class="nav-group">
      <a href="conferences.html" class="nav-link">Conferences</a>
      <a href="educational.html" class="nav-link">Educational</a>
      <a href="contact.html" class="nav-link">Contact Us</a>
    </div>
  </nav>

  <img src="banner.png" alt="Banner Image" class="banner" />
</div>

</body>
</html>
