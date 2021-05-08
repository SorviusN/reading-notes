# Class 05 Reading notes

# Topics for HTML/CSS Book:
- Images (94 - 125)
- Color (246 - 263)
- Text (264 -299)

## Images
- Picking which image to use. 
- Show an image at the right size.
- Optimize an image for use on the web.
- All images can be subject to copyrght.

### Storing images 
- Create a separate folder for all images present on a website.
- Create individual folders based on where the image will be on the website.

### Adding Images
- src is used to tell browser where to find the image file.
- alt provides alternate text in case
- title attribute for additional information about the image.
- width and height provide dimensions.

### Where to place images?
- Before a paragraph
- Inside start of paragraph
- In the middle of paragraph

### Image Sizing
- When sizing image, always set dimensions in terms of pixels.
- Vector images differ from bitmap images. They are created by placing points on grid, and drawing lines between points.

## Color

### Foreground and Background color
- Can express color in 3 different ways:
  - Rgb Value (rgb(0, 0, 0))
  - Hex Code (#111111)
  - Color names (blue)
  - use the /* */ to comment inside of CSS.
  -background color defines the color outside of any child elements.

### Contrast, Opacity
- Opacity defines how opaque your container is (Also called the alpha value)
- Contrast gives more or less color between the text and background.

### HSL
- Stands for Hue, Saturation, Light.
  - Hue is expressed as an angle (0 - 360)
  - Saturation is expressed as percentage
  - light is expressed as percentage with 0% white, 100% black.
- Used with newer version of CSS.
- an alternative way to give color to a page.


## Blog Post:
- JPEG vs PNG vs GIF

### TLDR
-JPEG Formats for images containing natural scenes, where color variety is smooth.
- PNG Format for transparency in images, or images that have sharp contrast like logos for companies. PNG is lossless.
- GIF for animations.

### Compression
- almost all forms of data is compressed to reduce siza and faster transmission.
- Two types of compression:
  - lossless means that it is possible to reconstruct original image from compressed because no info is lossed.
  - lossy means data is being lossed through compression.
