# Lecture Notes 11

## Topics for HTML/CSS Book:
- Images (406 - 427)
- Practical Info (476 - 492)

## Images
- Controlling size and alignment of your images with css keeps rules that affect presentation of your page.
- specify size and alignment of an image using CSS
- add background images to boxes
- create image rollovers

### Controlling Image Size
- use the width and height property, juts like a div.
- specifying height and width helps pages to load smoothly because code will load before images generally.

### Aligning images using css
- float property is added to the class that represents size of the image.
- By default, images are inline elements. This means that they flow within surrounding text.
- on containing element, you can use text align property with value of center.

### Background images
- allows you to place an image behind any HMTL element. could be entire or part of the page. 
- By default, background image will repeat to fill entire box.
- repeating images can be specified with no-repeat or repeat, also repeat-x and repeat-y

### Image rollovers and sprites
- It is possible to create a link/button that changes toa  second style when a user moves their mouse over. 
- Achieved by setting BG image for the link or button that has 3 different styles.
- when a single image is used for several different parts of an interface, it's called a sprite.

### Gradients
- being able to specify gradients is another useful tool for background images.
- need to specify two colors with linear gradient.

``` css
background-image: -moz-linear-gradient(#336666, #66cccc); // Firefox
background-image: -webkit-gradient(linear, 0%, 0%, 0% 100%, from(#66cccc, to(#336666)); // Safari
```

## Practical Info 
- Search engine optimization
- analytics for visitors
- putting sites on the web

### SEO (Serach engine optimization)
- Basics
  - The practice of trying to help your site appear nearer to the top of search engine results when people look for the topics that are covered in your websites.
- On page techniques:
  - methods you can use on your page to improve rating.
  - main component is looking at keywords that people are likely to enter into a search engine.
  - engines rely heavily on the text that is in your pages, so it is important that the terms people are going to search for are in text.
- Off page techniques
  - Get other sites to link to you
  - Search engines look at the words between the opening/closing a tag in the link. If the text in link contains the keywords it may be considered more relevant.

### Domain Names
- A lot of sites that offer domain name registration also offer web hosting
- domain name is your web address. There are many websites that allow you to register domain names.
- Server-side languages and databases
  - If you are using a content management system, it iwll likely use server-side programming language/database (php with MySQL DB or ASP Net with SQL server database).
