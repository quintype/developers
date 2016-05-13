# Sample App Question

You are required to build a simple one screen news app.

This app fetches configuration and stories from our API, and renders them in a UI indentical to YouTube.com (see attached screenshots). You may use any framework and programming language of your choice, and we'll expect working code and CSS.

This exercise should take roughly 3 hours for the code and project setup, and 4 hours for the front end development.

### Relevant APIs

You can find our APIs documented in [swagger format](https://itsman.quintype.com/sketches-swagger.json). Please note the API host is http://sketches.quintype.com

The relevant APIs are:
* /api/v1/stories for getting the stories for display
* /api/v1/config for getting the content to show in the menu

### Responsive Design

The app has three views, Desktop, Tablet and Phone. You are required to build the app to be responsive to a minimum of two of these screen sizes.

### Images

A hero image's URL can be found by appending the "hero-image-s3-key" to "http://quintype-01.imgix.net/". For example, the hero image whose s3 key is "quintype-demo/1234/foo.png" is "http://quintype-01.imgix.net/quintype-demo/1234/foo.png"

### Screenshots

![Phone View](./phone.png?raw=true "Phone View")
![Tablet View](./tablet.png?raw=true "Tablet View")
![Desktop View](./desktop.png?raw=true "Desktop View")
