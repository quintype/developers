# Images

Quintype currently uses [Imgix](https://www.imgix.com) to display images in various aspect ratios.

### base url

A image's URL can be obtained by appending the *"image-s3-key"* to "http://quintype-01.imgix.net/". For example, the hero image whose s3 key is "quintype-demo/1234/foo.png" is "http://quintype-01.imgix.net/quintype-demo/1234/foo.png". This is the image in it's original resolution, and can be transformed using any of [Imgix's Transforms](https://docs.imgix.com).

### focus point

Our editor allows the placement of a focus point on any image. The placement of a focus point guarantees that that point is always present in the viewport when the image is cropped, across different aspect ratios.

It is recommended that the focus point is used in conjuncture with the *picture* spec of HTML5, in order to show images at different aspect ratios on different devices. Using an `object-fit: cover;` will further center the image.

The refrence implementation for the focus point algorithm can be found in the [javascript implementation](https://github.com/quintype/quintype-js/blob/master/lib/focused_image.js).

The focus final image url can be calculated with the following pseudo code (for a 16x9 image with final width 640)

```js
var FocusedImage = require("quintype-js").FocusedImage;
var image = new FocusedImage('quintype-demo/1234/foo.png', metadata);
var output_url = "http://quintype-01.imgix.net/" + image.path([16, 9], {w: 640});
```
