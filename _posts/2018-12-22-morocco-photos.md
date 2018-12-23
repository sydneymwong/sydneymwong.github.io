---
layout: post
category: staging
title: "Morocco Photos"
date: 2018-12-22
---

<div>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}
.mySlides1, .mySlides2 {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a grey background color */
.prev:hover, .next:hover {
  background-color: #f1f1f1;
  color: black;
}
</style>
</head>
<body>

<h2 style="text-align:center">Pictures by Category</h2>

<p>Food:</p>
<div class="slideshow-container">
  <div class="mySlides1">
    <div class="numbertext">1 / 3</div>
    <img src="{{site.url}}/assets/morocco_photos/soup_msemen_dates.JPG" style="width:75%">
    <div class="text">harira, oat soup, msemen, dates</div>
  </div>

  <div class="mySlides1">
    <div class="numbertext">2 / 3</div>
    <img src="{{site.url}}/assets/morocco_photos/rice_vegetables.JPG" style="width:75%">
    <div class="text">rice with vegetables - a restaurant in Tagazhout made this for me</div>
  </div>

  <div class="mySlides1">
    <div class="numbertext">3 / 3</div>
    <img src="{{site.url}}/assets/morocco_photos/msemen.JPG" style="width:75%">
    <div class="text">msemen</div>
  </div>

  <a class="prev" onclick="plusSlides(-1, 0)">&#10094;</a>
  <a class="next" onclick="plusSlides(1, 0)">&#10095;</a>
</div>

<p>Our Neighborhood in Agadir:</p>
<div class="slideshow-container">
  <div class="mySlides2">
    <div class="numbertext">1 / 3</div>
    <img src="{{site.url}}/assets/morocco_photos/apartment.JPG" style="width:75%">
    <div class="text">our apartment</div>
  </div>

  <div class="mySlides2">
    <div class="numbertext">2 / 3</div>
    <img src="{{site.url}}/assets/morocco_photos/neighborhood_houses.JPG" style="width:75%">
    <div class="text">nice houses in our neighborhood</div>
  </div>

  <div class="mySlides2">
    <div class="numbertext">3 / 3</div>
    <img src="{{site.url}}/assets/morocco_photos/donkey.JPG" style="width:75%">
    <div class="text">our neighborhood donkey (this photo was taken from the doorstep of our apartment)</div>
  </div>

  <a class="prev" onclick="plusSlides(-1, 1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1, 1)">&#10095;</a>
</div>

<script>
var slideIndex = [1,1];
var slideId = ["mySlides1", "mySlides2"]
showSlides(1, 0);
showSlides(1, 1);

function plusSlides(n, no) {
  showSlides(slideIndex[no] += n, no);
}

function showSlides(n, no) {
  var i;
  var x = document.getElementsByClassName(slideId[no]);
  if (n > x.length) {slideIndex[no] = 1}    
  if (n < 1) {slideIndex[no] = x.length}
  for (i = 0; i < x.length; i++) {
     x[i].style.display = "none";  
  }
  x[slideIndex[no]-1].style.display = "block";  
}
</script>

</body>
</html> 
</div>