## Ch 16 Images

### Controling the Size of Images
- Common way is to creat a class of images; small, medium, and large and use height/width to define:
```html
<img src="image location" class="large">
```
```css

img.large { width: 500px; height: 500px;}

img.medium { width: 250px; height: 250px;}

img.small {width: 100px; height: 100px; }
```

### Aligning Images
- A more common way of aligning images is to specify a class for image-alignment and image-size and use the float property with margin for space between picture and text 
```html
<p><img src="image source" alt="image description' class="align-left medium">
```
```css
img.align-left { float: left; margin-right: 10px; }
img.medium {width: 250px; height: 250px; }
```

### Centering images
- images are inline by default; thus they flow within the surrounding text
- to center an image it should be turned into a **block level element**
- once in a block level element, 2 ways to horizontally center an image:
    - On **containing element**, use the `text-align: center;`
    - on the **image** use the `margin` and set the left/right values to auto
```html
<p><img src="image source" alt="image description" class="align-center medium">
```
```css
img.align-center { display: block; margin: 0px auto; }
img.medium {width: 250px; height: 250px;
```

### Video and audio in html5

```javascript
<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```

#More video and audio sample code
```javascript
<div class="player">
  <video controls>
    <source src="video/sintel-short.mp4" type="video/mp4">
    <source src="video/sintel-short.webm" type="video/webm">
    <!-- fallback content here -->
  </video>
  <div class="controls">
    <button class="play" data-icon="P" aria-label="play pause toggle"></button>
    <button class="stop" data-icon="S" aria-label="stop"></button>
    <div class="timer">
      <div></div>
      <span aria-label="timer">00:00</span>
    </div>
    <button class="rwd" data-icon="B" aria-label="rewind"></button>
    <button class="fwd" data-icon="F" aria-label="fast forward"></button>
  </div>
</div>
```
