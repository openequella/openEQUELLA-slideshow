# openEQUELLA-slideshow
Web component that leverages openEQUELLA content in a configurable slideshow

The slideshow displays images from oEQ items.  To find the items to display, it leverages the search REST API of oEQ.

The slideshow allows 'in app' configuration of the search query to dynamically change the slideshow. Alternatively, the slideshow can be configured with a `search-query` property the handles the configuration.

For items with multiple images, the slideshow will iterate through all of them, displaying them one at a time.

To install the web component on a web page:
```javascript
<script src="https://some-hosted-site/oeq-slideshow.js"></script>
<div style="width:600;">
  <oeq-slideshow
    oeq-url="https://some-hosted-oeq-site/"
    search-query="/api/search?q=keyword%20query&start=0&length=10&order=name&reverse=false&info=attachment&showall=false&status=LIVE">
  </oeq-slideshow>
</div>
```

## Future goals
- Support audio files
- Support video files
- Display a caption (from a configurable metadata field)
- Display a link to directly go to the item whose content is being displayed
- Have the ability to pause the slideshow and update the metadata (which will be saved in oEQ) for the current piece of content
-
