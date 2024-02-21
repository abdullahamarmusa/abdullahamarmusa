<!-- Header -->
<h1 align="center">Hi 👋, I'm Abdullah Amar Musa.</h1>
<h3 align="center">A passionate frontend developer from Bangladesh.</h3>

<!-- Profile Views Counter -->
<p align="left"> <img src="https://komarev.com/ghpvc/?username=abdullahamarmusa&label=Profile%20views&color=0e75b6&style=flat" alt="abdullahamarmusa" /> </p>

<!-- GitHub Trophies -->
<p align="left"> <a href="https://github.com/ryo-ma/github-profile-trophy"><img src="https://github-profile-trophy.vercel.app/?username=abdullahamarmusa" alt="abdullahamarmusa" /></a> </p>

<!-- Connect with Me -->
<h3 align="left">Connect with me:</h3>
<p align="left">
    <!-- Add your social media icons/links here -->
</p>

<!-- Languages and Tools -->
<h3 align="left">Languages and Tools:</h3>
<p align="left"> 
    <!-- Your languages and tools icons here -->
</p>

<!-- GitHub Stats -->
<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=abdullahamarmusa&show_icons=true&locale=en&layout=compact" alt="abdullahamarmusa" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=abdullahamarmusa&show_icons=true&locale=en" alt="abdullahamarmusa" /></p>

<!-- My Educations & Certifications -->
<h1>My Educations & Certifications</h1>

<div id="gallery">
 <a href="https://www.credly.com/earner/earned/badge/3cd2b897-fa5b-40ab-9987-96f659f17a1e" <img src="https://images.credly.com/size/340x340/images/941fa490-a052-46ae-beff-1ac8e55c117f/image.png" alt="Image 1" onclick="openModal();currentSlide(1)" class="hover-shadow">
  <img src="https://images.unsplash.com/photo-1707343843598-39755549ac9a?q=80&w=1932&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Image 2" onclick="openModal();currentSlide(2)" class="hover-shadow">
  <img src="https://images.unsplash.com/photo-1704186776780-19672ed2019a?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Image 3" onclick="openModal();currentSlide(3)" class="hover-shadow">
  <!-- Add more images as needed -->
</div>

<!-- The Modal/Lightbox -->
<div id="myModal" class="modal">
  <span class="close cursor" onclick="closeModal()">&times;</span>
  <div class="modal-content">
    <div class="mySlides">
      <img src="image1.jpg" style="width:100%">
    </div>
    <div class="mySlides">
      <img src="image2.jpg" style="width:100%">
    </div>
    <div class="mySlides">
      <img src="image3.jpg" style="width:100%">
    </div>
    <!-- Add more slides as needed -->
    <!-- Next and previous buttons -->
    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>
  </div>
</div>

<!-- Script for gallery functionality -->
<script>
var slideIndex = 1;
showSlides(slideIndex);

// Next/previous controls
function plusSlides(n) {
  showSlides(slideIndex += n);
}

// Thumbnail image controls
function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  if (n > slides.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  slides[slideIndex-1].style.display = "block";
}

// Open the Modal
function openModal() {
  document.getElementById("myModal").style.display = "block";
}

// Close the Modal
function closeModal() {
  document.getElementById("myModal").style.display = "none";
}
</script>
