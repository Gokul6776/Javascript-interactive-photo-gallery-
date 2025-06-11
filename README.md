function upDate(previewPic) {
  console.log("Mouse over image");
  console.log("Image src: " + previewPic.src);
  console.log("Image alt: " + previewPic.alt);

  // Get the element with id "image"
  let displayDiv = document.getElementById("image");

  // Change background image and text
  displayDiv.style.backgroundImage = "url('" + previewPic.src + "')";
  displayDiv.innerHTML = previewPic.alt;
}

function undo() {
  console.log("Mouse out of image");

  // Get the element with id "image"
  let displayDiv = document.getElementById("image");

  // Reset background image and text
  displayDiv.style.backgroundImage = "url('')";
  displayDiv.innerHTML = "Hover over an image below to display here.";
}
