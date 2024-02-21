<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Abdullah Amar Musa - Portfolio</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f2f2f2;
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
    }

    h1, h3 {
      text-align: center;
      margin-top: 20px;
    }

    h3 {
      margin-top: 10px;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }

    .image {
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    .image:hover {
      transform: scale(1.05);
    }

    .modal {
      display: none;
      position: fixed;
      z-index: 1;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.9);
    }

    .modal-content {
      margin: auto;
      display: block;
      width: 80%;
      max-width: 600px;
    }

    .mySlides {
      display: none;
    }

    .close {
      color: white;
      position: absolute;
      top: 10px;
      right: 25px;
      font-size: 35px;
      font-weight: bold;
      transition: 0.3s;
    }

    .close:hover,
    .close:focus {
      color: #bbb;
      text-decoration: none;
      cursor: pointer;
    }
  </style>
</head>
<body>

<!-- Header -->
<h1>Hi 👋, I'm Abdullah Amar Musa.</h1>
<h3>A passionate frontend developer from Bangladesh.</h3>

<!-- Profile Views Counter and GitHub Trophies -->
<p align="center"> 
  <img src="https://komarev.com/ghpvc/?username=abdullahamarmusa&label=Profile%20views&color=0e75b6&style=flat" alt="abdullahamarmusa" /> 
</p>
<p align="center"> 
  <a href="https://github.com/ryo-ma/github-profile-trophy">
    <img src="https://github-profile-trophy.vercel.app/?username=abdullahamarmusa" alt="abdullahamarmusa" />
  </a>
</p>

<!-- Connect with Me -->
<h3>Connect with me:</h3>
<p align="center">
  <!-- Add your social media icons/links here -->
</p>

<!-- Languages and Tools -->
<h3>Languages and Tools:</h3>
<p align="center"> 
  <!-- Your languages and tools icons here -->
</p>

<!-- GitHub Stats -->
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=abdullahamarmusa&show_icons=true&locale=en&layout=compact" alt="abdullahamarmusa" />
</p>
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=abdullahamarmusa&show_icons=true&locale=en" alt="abdullahamarmusa" />
</p>

<!-- My Educations & Certifications -->
<h1>My Educations & Certifications</h1>

<div class="container">
  <div class="gallery">
    <img src="https://images.credly.com/size/340x340/images/941fa490-a052-46ae-beff-1ac8e55c117f/image.png" alt="Image 1" class="image" onclick="openModal();currentSlide(1)">
    <img src="https://images.credly.com/size/340x340/images/d41de2b7-cbc2-47ec-bcf1-ebecbe83872f/GCC_badge_DA_1000x1000.png" alt="Image 2" class="image" onclick="openModal();currentSlide(2)">
    <img src="https://images.credly.com/size/340x340/images/f4b9febb-69f6-46d8-8797-1e504ebfe0f8/GCC_badge_UX_1000x1000.png" alt="Image 3" class="image" onclick="openModal();currentSlide(3)">
    <img src="https://s3.amazonaws.com/coursera_assets/meta_images/generated/CERTIFICATE_LANDING_PAGE/CERTIFICATE_LANDING_PAGE~FQCNLXW8ZCZM/CERTIFICATE_LANDING_PAGE~FQCNLXW8ZCZM.jpeg" alt="Image 4" class="image" onclick="openModal();currentSlide(4)">
  </div>

  <!-- The Modal -->
  <div id="myModal" class="modal">
    <span class="close cursor" onclick="closeModal()">&times;</span>
    <div class="modal-content">
      <div class="mySlides">
        <img src="https://images.credly.com/size/340x340/images/941fa490-a052-46ae-beff-1ac8e55c117f/image.png" style="width:100%">
      </div>
      <div class="mySlides">
        <img src="https://images.credly.com/size/340x340/images/d41de2b7-cbc2-47ec-bcf1-ebecbe83872f/GCC_badge_DA_1000x1000.png" style="width:100%">
      </div>
      <div class="mySlides">
        <img src="https://images.credly.com/size/340x340/images/f4b9febb-69f6-46d8-8797-1e504ebfe0f8/GCC_badge_UX_1000x1000.png" style="width:100%">
      </div>
      <div class="mySlides">
        <img src="https://s3.amazonaws.com/coursera_assets/meta_images/generated/CERTIFICATE_LANDING_PAGE/CERTIFICATE_LANDING_PAGE~FQCNLXW8ZCZM/CERTIFICATE_LANDING_PAGE~FQCNLXW8ZCZM.jpeg" style="width:100%">
      </div>
    </div>
  </div>
</div>

<!-- Script for gallery functionality -->
<script>
  var slideIndex = 1;
  showSlides(slideIndex);

  function plusSlides(n) {
    showSlides(slideIndex += n);
  }

  function currentSlide(n) {
    showSlides(slideIndex = n);
  }

  function showSlides(n) {
    var i;
    var slides = document.getElementsByClassName("mySlides");
    var modal = document.getElementById("myModal");
    if (n > slides.length) {slideIndex = 1}    
    if (n < 1) {slideIndex = slides.length}
    for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
    }
    slides[slideIndex-1].style.display = "block";
  }

  function openModal() {
    document.getElementById("myModal").style.display = "block";
  }

  function closeModal() {
    document.getElementById("myModal").style.display = "none";
  }
</script>

</body>
</html>
