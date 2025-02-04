# PolicyPals Landing Page - Maintenance Guide

This guide will help you maintain and customize the PolicyPals insurance landing page. It's written for beginners with no prior coding experience.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
The header contains the company name and navigation menu. To update:

1. Company Name:
```html
<!-- Find this line in the header section -->
<span class="text-xl font-bold text-blue-500">PolicyPals</span>
```
- Replace "PolicyPals" with your desired company name
- `text-xl` controls text size
- `text-blue-500` controls text color

2. Navigation Menu Items:
```html
<a href="#features" class="text-gray-300 hover:text-white transition-colors duration-200">Features</a>
```
- Update text between `>` and `</a>`
- `text-gray-300` is the default color
- `hover:text-white` is the color when hovering

### Hero Section
Located at the top of the page with main heading and subheading:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight text-white mb-8">
    Policy Pals Find You The Friendliest Insurance Policies
</h1>
```
- `text-4xl`, `md:text-5xl`, `lg:text-6xl` control text size at different screen sizes
- `mb-8` adds margin bottom spacing
- Replace the text while keeping the classes intact

### Features Section
Each feature card follows this structure:
```html
<div class="bg-gray-900 rounded-2xl p-8 shadow-xl hover:shadow-2xl transition-all duration-300 transform hover:scale-105">
    <!-- Feature content -->
</div>
```
- `bg-gray-900` sets background color
- `p-8` adds padding
- `hover:scale-105` creates hover animation

## Fixing Broken Links

### Current Links Inventory:
1. Navigation Menu Links:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="https://PolicyPals.Co.Uk">Get Started</a>
```
To update:
- Internal links (starting with #) connect to page sections
- External links (starting with https://) go to other websites
- Replace "https://PolicyPals.Co.Uk" with your actual website URL

### Call-to-Action Buttons:
```html
<a href="https://PolicyPals.Co.Uk" class="inline-flex items-center justify-center px-8 py-4 text-lg">
    Find Your Perfect Policy
</a>
```
- Update the `href` attribute with your desired URL
- Keep the class attributes to maintain styling

## Linking Privacy and Terms Pages

### Footer Links
Locate this section in the footer:
```html
<div>
    <h3 class="text-sm font-semibold uppercase tracking-wider">Legal</h3>
    <ul class="mt-4 space-y-2">
        <li>
            <a href="#" class="text-gray-400 hover:text-white transition-colors duration-200">Privacy Policy</a>
        </li>
        <li>
            <a href="#" class="text-gray-400 hover:text-white transition-colors duration-200">Terms of Service</a>
        </li>
    </ul>
</div>
```

To add privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your website folder
2. Update the links:
```html
<a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-200">Privacy Policy</a>
<a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-200">Terms of Service</a>
```

## Troubleshooting

Common Issues:
1. **Broken Styles**
   - Make sure the Tailwind CSS CDN link is present in the head section
   - Check for typos in class names
   - Classes are case-sensitive

2. **Links Not Working**
   - Verify file names match exactly
   - Check for proper file location
   - Ensure URLs include "https://" for external links

3. **Responsive Design Issues**
   - Keep the responsive classes (`md:`, `lg:`, etc.)
   - Test on different screen sizes
   - Don't remove the viewport meta tag

Remember:
- Always make a backup before editing
- Test changes in a browser
- Check mobile responsiveness
- Validate links before publishing

Need help? Contact support@policypals.co.uk for assistance.