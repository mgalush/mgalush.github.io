# HTML Images

Specifying an image height and width helps the page load more smoothly because HTML and CSS will often load before the images and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download

Common immage sizes:
- Small portrait: 220 x 360
- Small landscape: 330 x 210
- Feature photo: 620 x 400

Determine what sizes will be commonly used across the site and label with `small`, `medium`, and `large` for easy styling in CSS

When setting the `background-image` to `repeat`, use a small tile image since a background image is the last thing to load on a page and a large image can slow down the webpage.  You can `repeat-`, `repeat-x`, set to `fixed` or `scroll`, or set to `no-repeat`

If not repeating, the `background-position` will let you specify where you want the image to reload. You can use built in positions such as `left top`, `left center` or `right bottom`.  If you only specify one value, the second value will default to `center`.  You can also pixels or percentage, which will represent the distance from the top left corner of the window.  For example: to place the image top left, you would set `background-position: 0% 0%;` and to center the image you would set `background-position: 50% 50%;`

You can set all of these attributes using the `background` property which takes in the following:
1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position

# SEO

Search Engine Optimization is the practice of trying to help your site appear nearer the top of search engine results. 

There are 7 key places where keywords can appear in order to improve SEO:
1. Page title
2. URL / Web address
3. Headings
4. Text
5. Link text
6. Image alt text
7. Page descriptions

In order to put your website on the internet, you will need a domain name and web hosting. 

To transfer files your code and images to your hosting company, you will use a **File Transfer Protocol** which allow you to transfer files from your local computer to a web server
