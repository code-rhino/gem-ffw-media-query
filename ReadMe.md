# Transcript 

[Video Link](https://vimeo.com/user214919587/review/909179299/249cc18484)

Creating responsive designs with media queries is essential for accommodating various screen sizes, from desktops to mobile devices. This step-by-step guide will walk you through the process of using media queries to adjust the style of a webpage so it remains visually appealing across different devices, focusing on adjusting the font size of a heading element.

### Step 1: Setup the HTML Structure
Begin with an HTML file that includes a `div` element with the class `content`, containing an `h1` heading and a paragraph `p`. This structure is the foundation for applying responsive styles.

```html
<div class="content">
    <h1>My Big Title</h1>
    <p>This text may look great on larger screen sizes, however on smaller screens like mobile phones it can be a bit much.</p>
</div>
```

### Step 2: Add Base CSS Styles
Link a CSS file to your HTML document and set base styles for the `h1` element within the `.content` class. These styles are applied by default, optimized for desktop or larger screen sizes.

```css
.content h1 {
    font-size: 100px; /* Default font size for desktop */
    line-height: 1.2; /* Default line height */
    margin-bottom: 30px; /* Default bottom margin */
    padding: 0 20px; /* Default padding */
}
```

### Step 3: Implement Media Queries for Responsive Design
Add a media query to adjust the styles of the `h1` element when the webpage is viewed on screens smaller than 600 pixels wide. This is where you customize the font size, line height, margin, and padding for smaller devices.

```css
@media (max-width: 600px) {
    .content h1 {
        font-size: 24px; /* Reduced font size for small screens */
        line-height: 1.3; /* Adjusted line height for better readability */
        margin-bottom: 20px; /* Adjusted bottom margin */
        padding: 0 15px; /* Adjusted padding */
    }
}
```

### Step 4: Test Responsiveness
- **On Desktop:** The heading will display with a font size of 100px, adhering to the base style.
- **On Mobile Devices (or any screen under 600px wide):** The heading's font size will reduce to 24px, making it more suitable for smaller screens without compromising the design integrity.

### Step 5: Fine-Tuning Font Size
To ensure the text remains on one line on smaller screens without breaking or looking disproportionate, you might need to experiment with the font size. Use developer tools in a browser to dynamically adjust the font size and find the ideal size that fits your design requirements. For this example, after testing, it was determined that a font size of 24px works well for screens smaller than 600 pixels wide.

### Step 6: Save and Verify Changes
After adjusting the media query in your CSS file, save the changes and refresh your webpage. Use developer tools or resize your browser window to test the responsive design across various screen sizes, ensuring the heading adjusts correctly according to the screen width.

### Conclusion
Media queries are a powerful tool for creating responsive designs, allowing you to tailor your website's appearance to ensure optimal readability and user experience across all devices. By adjusting properties like font size, line height, and margins based on screen size, you can maintain the intended design aesthetic and improve accessibility for your audience.