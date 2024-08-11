### **README.md for Hosting a Custom Font on GitHub**

---

# **Custom Font Hosting Repository**

This repository hosts the custom font files that can be used in your web projects. The fonts are stored in various formats to ensure compatibility across different browsers.

## **Font Files Included**
- `font.woff2`: Web Open Font Format 2 (WOFF2) – Recommended for modern browsers.
- `font.woff`: Web Open Font Format (WOFF) – Widely supported format for web fonts.
- `font.ttf`: TrueType Font (TTF) – Supported by most browsers and platforms.

## **Using the Custom Font in Your Project**

Follow these steps to use the custom font hosted in this GitHub repository in your web project:

### **1. Get the Raw URL of the Font Files**

To use the font in your CSS, you need to obtain the direct raw URL for each font file.

1. Navigate to the font file you want to use (e.g., `font.woff2`).
2. Click on the file to open it.
3. Click on the "Raw" button to get the direct link to the file.
4. Copy the URL, which will look something like this:

   ```
   https://raw.githubusercontent.com/username/repository/branch/font.woff2
   ```

### **2. Add the `@font-face` Rule in Your CSS**

Use the `@font-face` rule in your CSS file to define the custom font. Here's an example of how to do this:

```css
@font-face {
    font-family: 'OpenSauceSans';
    src: url('https://raw.githubusercontent.com/gauravshharma/Custom-font-Open-Sauce/font/font.woff2') format('woff2'),
         url('https://raw.githubusercontent.com/gauravshharma/Custom-font-Open-Sauce/font/font.woff') format('woff'),
         url('https://raw.githubusercontent.com/gauravshharma/Custom-font-Open-Sauceb/font/font.ttf') format('truetype');
    font-weight: normal;
    font-style: normal;
}
```

### **3. Apply the Font to Your Website**

Once the font is defined using the `@font-face` rule, you can apply it to HTML elements in your CSS file:

```css
body {
    font-family: 'OpenSauceSans', sans-serif;
}
```

### **4. Fallback Fonts**

For better user experience, include fallback fonts in case the custom font fails to load:

```css
body {
    font-family: 'OpenSauceSans', Arial, sans-serif;
}
```

### **5. Test and Validate**

Ensure the font is loading correctly across different browsers and devices. Verify that the font files are accessible via the raw GitHub URLs.

## **Contributing**

If you have suggestions for improving this repository or want to add more font files, feel free to fork the repository, make your changes, and submit a pull request.

## **License**

This repository is licensed under the MIT License. Please see the LICENSE file for more details.

---
