# Preview

### Technical Overview

The preview functionality is implemented with a combination of the backend editor, and the front end UI. The front end page has to implement two routes. `/preview/story` and `/preview/home`. The editor fetches this page via either HTTP or HTTPS, then served in an IFrame on the editor (via HTTPS). As the story is updated in the editor, the story is passed to the page via the message API, and the page is expected to rerender on the Front End.

### HTTPs Only

As the content is loaded via HTTPS, any HTTP content (external JS, etc...) will not render.

### Example

Below is sample code explaining how to listen via the IFrame message API.

```javascript
var StoryPreview = (function() {
  window.addEventListener("message", function(event){
  var template = Liquid.parse("{% include 'pages/story' %}");
  var story = event.data['story'];
    if (story) {
      $("#story-preview").html(template.render({story: story, preview: true}));

      // Do other things to make the page work correctly, such as post load JS
    }
  });
});
```
