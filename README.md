Head Section:
Meta Tags:
Sets the character encoding (UTF-8) and specifies the viewport for responsive design (width=device-width, initial-scale=1.0).
Title and External Resources:
Sets the title of the document to "Photo Editor".
Imports the Font Awesome library for icons (https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css).
Internal Styles:
Defines styles for the body background, header (h1), and container (mycontainer).
Uses the Google Fonts API ('Indie Flower') for a specific font style.
Defines the layout for the canvas and buttons (button), including their appearance, sizing, colors, and hover effects.
Body Section:
Header (myheader):
Displays a centered header with a camera icon (fa fa-camera-retro) using Font Awesome and a title ("Photo Editor") styled with a custom font.
Main Container (mycontainer):
Uses a grid layout (display: grid) with two columns (grid-template-columns: 70% 30%) to arrange elements.
Canvas (canvasContainer):
Contains a canvas element (canvas) for displaying and editing images.
Styled with a fixed width and height (width: 700px; height: 500px;) and a border (border-style: inset;) for image display and manipulation.
Button Panel:
Contains a list (ul) of buttons (button) for different photo editing functions:
Upload Image: Allows users to upload an image file (<input type="file" id="uploadInput" accept="image/*">).
Grayscale, Black & White, Vintage, Contrast: Buttons to apply different image filters.
Reset: Button to revert to the original uploaded image.
Save: Button to save the edited image as a PNG file.
JavaScript Functionality (script):
Event Listeners:
Image Upload: Handles image upload and displays the image on the canvas using FileReader and ctx.drawImage().
Save Button: Converts the canvas content to a data URL (canvas.toDataURL()) and allows users to download the edited image (a.click()).
Reset Button: Resets the canvas to display the original uploaded image stored in originalImage.
Filter Functions:
Grayscale, Black & White, Vintage, Contrast: Functions (applyFilter) to manipulate the image data (ctx.getImageData) based on selected filters (grayscale, blackWhite, vintage, contrast).
Each filter modifies the image's pixel data (imageData.data) to achieve the desired effect and updates the canvas (ctx.putImageData).# Image-Editor-Mini-Project
