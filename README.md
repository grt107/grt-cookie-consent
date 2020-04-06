# GRT Cookie Consent - jQuery Plugin
Simple and lightweight jQuery plugin used for Cookie Consent on GDPR Law

You can check the demo here: [grt107.github.io/grt-cookie-consent/](http://grt107.github.io/grt-cookie-consent/)

# Screenshot:
![Alt text](/screenshot.jpg?raw=true "Demo Screenshot")

# How to use the plugin in your website:
1- Include the plugin stylesheet file ```grt-cookie-consent.css``` inside your ```<head>``` tag

  ```html
  <link rel="stylesheet" href="grt-cookie-consent.css">
  ```

2- Include the plugin javascript file ```grt-cookie-consent.js``` inside the ```<body>``` tag and after ```jquery.min.js```

  ```html
  <script src="grt-cookie-consent.js"></script>
  ```

3- Add the following code inside your document  ```body``` and change the text content and button name:

  ```html
	<div class="grt-cookie"> 
	 <div class="grt-cookies-msg">
	 <p> We use cookies to ensure that we give you the best experience on our website. If you continue to use this site we will assume that you accept and understand our <a href="">Privacy Policy</a>, and our <a href="">Terms of Service</a>. </p> </div> 
	 <span class="grt-cookie-button">Accept</span>
	</div>
  ```

4- Initialize the plugin with default values at the end of all javascript files using the code below (after ```jquery.min.js``` and ```grt-cookie-consent.js```)

```html
  <script> $(".grt-cookie").grtCookie(); </script>
  ```

# Advanced Options
You can modify plugin colors and cookie duration by using the following code:

  ```html
	<script>
	$(".grt-cookie").grtCookie({
		// Main text and background color
		textcolor: "#333",
		background: "#fff",
		// Button colors
		buttonbackground: "#c40b14",
		buttontextcolor: "#fff",
		// Duration in days
		duration: 365,
	});
 	</script>
  ```