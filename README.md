# PondFountainDepot Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the PondFountainDepot landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Location: Line 19 (Announcement Bar) -->
<p>Fast Worldwide Shipping (5 days delivery) | Free Returns</p>

<!-- Location: Line 24 (Company Name) -->
<a href="/" class="text-2xl font-bold text-blue-600">PondFountainDepot</a>
```
To modify text content:
1. Locate the specific section in the HTML
2. Change the text between the opening and closing tags
3. Maintain any existing HTML tags

#### Hero Section
```html
<!-- Location: Lines 45-47 -->
<h1 class="text-4xl md:text-6xl font-bold text-white mb-6 leading-tight">Premium Pond Fountains & Aeration Systems</h1>
<p class="text-xl md:text-2xl text-white/90 mb-8">Boost Pond Health & Beauty | Premium Fountains & Aeration</p>
```

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:` prefix indicates styles apply only on medium screens and larger
- Example: `text-4xl md:text-6xl` means:
  - Mobile: text is extra-large (4xl)
  - Desktop: text is super-large (6xl)

#### Common Class Patterns
```html
<!-- Button Styling Example -->
<button class="bg-blue-600 text-white px-6 py-3 rounded-full hover:bg-blue-700 transition duration-300">
```
- `bg-blue-600`: Background color
- `text-white`: Text color
- `px-6`: Horizontal padding
- `py-3`: Vertical padding
- `rounded-full`: Rounded corners
- `hover:bg-blue-700`: Color change on hover
- `transition duration-300`: Smooth transition effect

## Fixing Broken Links

### Navigation Menu Links
Current placeholder links in the header:
```html
<!-- Location: Lines 26-28 -->
<a href="#" class="text-gray-600 hover:text-blue-600 transition duration-300">Products</a>
<a href="#" class="text-gray-600 hover:text-blue-600 transition duration-300">Solutions</a>
<a href="#" class="text-gray-600 hover:text-blue-600 transition duration-300">About</a>
```

To update links:
1. Replace `#` with proper URLs
2. Example:
```html
<a href="/products.html" class="text-gray-600 hover:text-blue-600 transition duration-300">Products</a>
```

### Footer Links
```html
<!-- Location: Lines 181-185 -->
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Products</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">About Us</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Contact</a></li>
</ul>
```

## Adding Privacy and Terms Pages

### Footer Modification
Add these links to the Quick Links section in the footer:

```html
<!-- Add after existing footer links -->
<li><a href="/privacy.html" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
<li><a href="/terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
```

### Complete Footer Links Section
```html
<div>
    <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
    <ul class="space-y-2">
        <li><a href="/products.html" class="text-gray-400 hover:text-white transition duration-300">Products</a></li>
        <li><a href="/about.html" class="text-gray-400 hover:text-white transition duration-300">About Us</a></li>
        <li><a href="/contact.html" class="text-gray-400 hover:text-white transition duration-300">Contact</a></li>
        <li><a href="/privacy.html" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
        <li><a href="/terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
    </ul>
</div>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Images**
   - Check image URLs in the `src` attributes
   - Ensure images exist in the correct directory
   - Verify image paths are relative to the HTML file

2. **Responsive Design Issues**
   - Test different screen sizes using browser dev tools
   - Verify `md:` classes are properly applied
   - Check container widths and padding

3. **Link Problems**
   - Confirm all HTML files exist in the correct location
   - Use relative paths (e.g., `/about.html`) for internal links
   - Use full URLs (e.g., `https://example.com`) for external links

### Need Help?
- Check the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Verify HTML syntax using [W3C Validator](https://validator.w3.org/)
- Test responsive design using Chrome DevTools (F12)

Remember to always backup your files before making changes and test all modifications in a development environment first.