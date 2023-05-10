# Using Images in HTML

## Images in HTML

### How Do We Put an Image on a Webpage

- In order to put a simple image on a web page, we use the img element
- This is a void element that requires two attributes to be useful: src and alt
- The src attribute contains a URL pointing to the image you want to embed in the page
- As with the href attribute for a elements, the src attribute can be a relative URL or an absolute URL
- Without a src attribute, an img element has no image to load

#### Alternative Text

- alt is a value that is supposed to be a textual description of the image, for use in situations where the image cannot be seen/displayed or takes a long time to render because of a slow internet connection
- Why you need alt text:
  - The user is visually impaired, and is using a screen reader to read the web out to them
  - the spelling of the file or path name might be wrong
  - The browser doesn't support the image type
  - You may want to provide text for search engines to utilize
  - Users have turned off images to reduce data transfer volume and distractions

#### Width and Height

- You can use the width and height attributes to specify the width and height of your image
- You shouldn't alter the size of your images using HTML attributes

#### Image Titles

- You can also add title attributes to images, to provide further supporting information if needed
- Title has a number of accessibility problems, mainly based around the fact that screen reader support is very unpredictable and most browsers won't show it unless you are hovering with a mouse

### Annotating Images with Figures and Figure Captions

- There are a number of ways that you could add a caption to go with your image