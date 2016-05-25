##Dependencies
ScrollSprite's only dependency is on jQuery.
##Installation
Include jquery.sprite-scroll.js in your document and instantiate a new SpriteScroll object.

Example:
```
var soda = new SpriteScroll({
  width: 152,
  height: 270,
  rowlength: 4,
  frames: 10,
  sprite: "..path/to/image/file",
  elementId: 'bottle',
  scrollBounds: 920,
  scrollSpeed: 24
});```

## Options
Name | Type | Description
--- | --- | ---
width | int | The pixel width of an individual sprite
height | int | The pixel height of an individual sprite
rowlength | int | The number of frames in each row of your spritesheet
frames | int | The total number of frames in your spritesheet
sprite | string | The path or URL to your sprite sheet
elementId | string | The ID of the element that will be holding the sprite sheet
scrollBounds | int | How far down the page the animation should be run. This is to minimize calls to animate outside of the animation viewport.
scrollSpeed | int | The number of scrollTop units to go by before moving to the next frame.
debug | boolean | If set to true, output debug information to the console.
