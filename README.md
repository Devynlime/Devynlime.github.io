# Vue Image Switcher

This is an image switcher built with Vue.js. Users can click buttons to switch the displayed image, and each image has a corresponding description text.

## Implementation Logic

In the HTML, we have a root element of the Vue application, which has an id of `app`. Inside this element, we have a `.content-container` that contains the buttons and the image.

The buttons are in a .button-container, which contains three image buttons. Each button has a `v-on:click` directive that changes the value of `currentImage` when the user clicks the button.

The image is in an .image-container, which contains an image element and three .overlay elements. The src attribute of the image element is bound to images`[currentImage]`, so when the value of `currentImage` changes, the displayed image also changes. The .overlay elements are the description texts of the image, they use the v-if directive to show or hide based on the value of `currentImage`.

In the CSS, we use Flexbox layout to arrange the child elements of .content-container (i.e., the buttons and the image). We also use CSS animation to implement the blinking effect of the .overlay elements.

## Usage

Open the index.html file in a browser to view the effect.

Click the buttons to switch the image. Each image has a corresponding description text that blinks above the image.

### Notes

Make sure your browser supports Vue.js and CSS animations.
If you want to change the images or description texts, you need to modify the data option of the Vue instance and the content of the .overlay elements.
If you want to change the layout or styles, you need to modify the CSS rules.
