<h1 align="center">
<!--   <img src="https://cdn.sparkfun.com/assets/home_page_posts/2/3/2/6/arm_logo.png" width="250"> -->
  <br>
  Masonry Portfolio
</h1>

<h3>A static masonry like portfolio with vanilla JS, CSS and HTML.</h3>
The website is fully responsive, adding content is as easy as adding elements to a JSON file and elements are added to the DOM only when necessary.

<h2>Why static?</h2>

In order to publish the portfolio to github pages everything had to be done static.
This restriction however has not inhibitted any of the features that I had in mind (infinite scroll, modals, etc).

<h2>Infinite scroll with static pages?</h2>

In order to achieve a infinite scroll an IntersectionObserver() was used. When the footer is visible a fetch() request is made to a .json file with the images to load, content for the modal and title.

The JSON file has the following content:
````
[
  {
    "content":"Title for the hover and modal",
    "img":"route/to/the/image.jpg",
    "html":"HTML for the modal"
  }
]
````
