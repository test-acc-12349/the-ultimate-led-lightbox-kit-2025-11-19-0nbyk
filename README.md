# LED Lightbox Kit Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain and customize your LED Lightbox Kit landing page. Whether you're new to web development or looking for a quick reference, this documentation covers everything you need to know about updating your site.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Updating Text Content](#updating-text-content)
3. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
4. [Managing Links](#managing-links)
5. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
6. [Common Customizations](#common-customizations)
7. [Troubleshooting](#troubleshooting)

---

## Getting Started

### What You'll Need

- A text editor (we recommend: VS Code, Sublime Text, or even Notepad++)
- Your `index.html` file
- Basic understanding of HTML tags and how they work
- No coding experience required!

### File Structure

Your landing page uses a single HTML file with embedded CSS and JavaScript. Here's the basic structure:

```
index.html (contains everything)
├── CSS Styles (in <style> tags)
├── HTML Content (in <body> tags)
└── JavaScript (in <script> tags)
```

### How to Edit Your File

1. **Right-click** on `index.html` and select "Open with" → Choose your text editor
2. **Locate** the section you want to edit using `Ctrl+F` (or `Cmd+F` on Mac)
3. **Make your changes** carefully
4. **Save** the file using `Ctrl+S` (or `Cmd+S` on Mac)
5. **View changes** by refreshing your browser

---

## Updating Text Content

### Understanding HTML Structure

Text content on your landing page is organized in logical sections. Each section is wrapped in HTML tags that define its purpose. Here's how to find and update text:

### Section 1: Announcement Bar (Top of Page)

**Location:** Lines 88-91

**Current Text:**
```html
<p class="text-sm font-medium">🚚 Fast Worldwide Shipping (5 days delivery) | 100% Satisfaction Guarantee</p>
```

**How to Update:**
1. Find the line starting with `<p class="text-sm font-medium">`
2. Replace the text between `>` and `</p>` with your message
3. Keep the emoji if you like it, or replace it with another

**Example - Change to:**
```html
<p class="text-sm font-medium">✨ Premium Quality | 30-Day Money Back Guarantee | Expert Support</p>
```

---

### Section 2: Header/Logo (Navigation Bar)

**Location:** Lines 96-98

**Current Text:**
```html
<a href="#" class="text-2xl font-bold text-gray-900 hover:text-blue-600 transition-colors duration-300">
    <i class="fas fa-lightbulb text-blue-600 mr-2"></i>LPK
</a>
```

**How to Update:**
1. Find the text `LPK` (this is your logo text)
2. Replace `LPK` with your company name
3. The lightbulb icon (`fas fa-lightbulb`) can stay or be replaced

**Example - Change to:**
```html
<a href="#" class="text-2xl font-bold text-gray-900 hover:text-blue-600 transition-colors duration-300">
    <i class="fas fa-lightbulb text-blue-600 mr-2"></i>My Studio Pro
</a>
```

---

### Section 3: Hero Section (Large Title & Subtitle)

**Location:** Lines 153-161

**Current Text:**
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl font-bold text-white mb-6 leading-tight tracking-tight">
    The Ultimate LED Lightbox Kit
</h1>
<p class="text-xl sm:text-2xl md:text-3xl text-gray-100 mb-8 font-light leading-relaxed">
    Professional Photography Equipment for Studio Quality Results
</p>
```

**How to Update:**
1. Replace the text inside `<h1>` tags with your main headline
2. Replace the text inside the `<p>` tags with your subtitle
3. Keep the HTML tags, only change the text

**Example - Change to:**
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl font-bold text-white mb-6 leading-tight tracking-tight">
    Professional Lighting for Every Creator
</h1>
<p class="text-xl sm:text-2xl md:text-3xl text-gray-100 mb-8 font-light leading-relaxed">
    Affordable, Portable, Studio-Quality Results
</p>
```

---

### Section 4: Features Section (Three Cards)

**Location:** Lines 183-225

The Features section contains three cards with icons, titles, and descriptions. Each card has this structure:

```html
<div class="feature-card bg-gradient-to-br from-blue-50 to-blue-100 p-8 rounded-2xl border border-blue-200 hover:shadow-xl">
    <div class="mb-6 flex items-center justify-center w-16 h-16 bg-blue-600 rounded-full">
        <i class="fas fa-camera text-white text-2xl"></i>
    </div>
    <h3 class="text-2xl font-bold text-gray-900 mb-3">Professional Photography</h3>
    <p class="text-gray-700 leading-relaxed">
        [Feature description goes here]
    </p>
</div>
```

**How to Update Each Feature Card:**

1. **Find the feature card** you want to change (search for the title)
2. **Update the title** - Replace text in `<h3>` tags
3. **Update the description** - Replace text in `<p>` tags
4. **Change the icon** - Replace the icon class (see Icon Reference below)

**Feature Card 1 - Professional Photography:**
- **Title location:** Line 193
- **Description location:** Lines 194-197
- **Icon location:** Line 189 (`fas fa-camera`)

**Feature Card 2 - Portable Setup:**
- **Title location:** Line 208
- **Description location:** Lines 209-212
- **Icon location:** Line 204 (`fas fa-briefcase`)

**Feature Card 3 - Energy Efficient:**
- **Title location:** Line 223
- **Description location:** Lines 224-227
- **Icon location:** Line 219 (`fas fa-leaf`)

**Example - Update Feature 1:**
```html
<h3 class="text-2xl font-bold text-gray-900 mb-3">Advanced LED Technology</h3>
<p class="text-gray-700 leading-relaxed">
    Our cutting-edge LED system delivers perfect color accuracy for every shot. 
    Ideal for all photography styles and professional productions.
</p>
```

---

### Section 5: Benefits Section (Three Detailed Sections)

**Location:** Lines 242-340

The Benefits section has three larger sections with images and detailed text. Each benefit has:
- A heading (`<h3>`)
- Detailed paragraphs (`<p>` tags)
- A bulleted list (`<ul>` with `<li>` items)

**Benefit 1 - Studio Quality Light:**
- **Heading location:** Line 252
- **Description paragraphs:** Lines 253-257
- **Bullet points:** Lines 258-268

**How to Update Bullet Points:**

Find the section with `<ul class="space-y-3">` and update each item:

```html
<ul class="space-y-3">
    <li class="flex items-center text-gray-700">
        <i class="fas fa-check-circle text-blue-600 mr-3 text-lg"></i>
        <span class="font-medium">Your updated text here</span>
    </li>
</ul>
```

**Example - Update a bullet point:**
```html
<li class="flex items-center text-gray-700">
    <i class="fas fa-check-circle text-blue-600 mr-3 text-lg"></i>
    <span class="font-medium">Perfect for Instagram & TikTok content</span>
</li>
```

---

### Section 6: Call-to-Action (CTA) Section

**Location:** Lines 345-365

**Current Text:**
```html
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-6 tracking-tight">
    Ready to Elevate Your Photography?
</h2>
<p class="text-lg md:text-xl text-blue-100 mb-8 leading-relaxed max-w-2xl mx-auto">
    Join thousands of professional photographers who trust our LED Lightbox Kit for their most important projects
</p>
```

**How to Update:**
1. Replace the heading text inside `<h2>` tags
2. Replace the paragraph text inside `<p>` tags
3. Update button text (see Button Text section below)

---

### Section 7: About Us Section

**Location:** Lines 377-430

The About section contains two main paragraphs with different background colors:

**Heritage Paragraph:**
- **Location:** Lines 386-391
- **Title:** "Our Heritage" (inside `<h3>`)
- **Content:** Inside `<p>` tags

**Mission Paragraph:**
- **Location:** Lines 393-398
- **Title:** "Our Mission & Values" (inside `<h3>`)
- **Content:** Inside `<p>` tags

**Stats Section:**
- **Location:** Lines 401-415
- Update numbers and labels in each stat box

**Example - Update Stats:**
```html
<div class="text-center p-6 bg-gray-50 rounded-xl">
    <div class="text-4xl md:text-5xl font-bold text-blue-600 mb-2">75K+</div>
    <p class="text-gray-700 font-semibold">Active Users</p>
</div>
```

---

### Section 8: Testimonials Section

**Location:** Lines 442-530

Each testimonial card contains:
- Star rating (automatic, don't change)
- Quote text
- Customer name
- Customer title

**How to Update a Testimonial:**

Find the testimonial you want to change and update:

```html
<p class="text-gray-700 text-lg leading-relaxed mb-6">
    "Your new testimonial text goes here. Keep the quotation marks."
</p>
```

And update the customer info:
```html
<p class="font-bold text-gray-900">New Customer Name</p>
<p class="text-gray-600 text-sm">New Customer Title</p>
```

Also update the initials circle:
```html
<div class="w-12 h-12 bg-blue-600 rounded-full flex items-center justify-center text-white font-bold mr-4">
    NC
</div>
```

---

### Section 9: FAQ Section

**Location:** Lines 541-620

Each FAQ item has:
- A question (in button)
- An answer (in hidden content)

**How to Update an FAQ:**

```html
<!-- Question -->
<button class="faq-toggle w-full px-6 md:px-8 py-5 md:py-6 flex items-center justify-between bg-gray-50 hover:bg-gray-100 transition-colors duration-300 text-left">
    <span class="text-lg md:text-xl font-semibold text-gray-900">Your question here?</span>
    <i class="faq-icon fas fa-chevron-down text-gray-600 text-lg"></i>
</button>

<!-- Answer -->
<div class="faq-content bg-white px-6 md:px-8 py-4 md:py-6 border-t border-gray-200">
    <p class="text-gray-700 text-lg leading-relaxed">
        Your detailed answer goes here.
    </p>
</div>
```

---

### Section 10: Contact Section

**Location:** Lines 627-705

**Form Labels and Placeholders:**
- Name input: Line 644
- Email input: Line 649
- Subject input: Line 654
- Message textarea: Line 659

**How to Update:**
```html
<!-- Change placeholder text (hint text) -->
<input type="text" id="name" name="name" placeholder="Your name here" ...>

<!-- Change label text -->
<label for="name" class="block text-sm font-semibold text-gray-700 mb-2">Your Full Name</label>
```

**Contact Information:**
- Email: Line 678 - `admin@lpk.com`
- Website: Line 684 - `https://lpk.com`

---

### Section 11: Footer

**Location:** Lines 710-800

**Company Info:**
- Description: Line 722-724
- Social media links: Lines 725-735

**Quick Links:**
- Location: Lines 738-747

**Support Links:**
- Location: Lines 750-759

**Contact Info:**
- Location: Lines 762-778

**How to Update Footer Text:**
1. Find the section you want to update
2. Replace text inside tags, keeping HTML structure intact
3. For links, update the `href="#"` attribute (see Links section below)

---

## Modifying Tailwind CSS Classes

### Understanding Tailwind CSS

Tailwind CSS is a utility-first framework that uses class names to style elements. Instead of writing CSS code, you add descriptive class names to HTML elements.

**Basic Format:**
```html
<div class="text-2xl font-bold text-blue-600 mb-4">
    Styled text
</div>
```

Breaking this down:
- `text-2xl` = Large text size
- `font-bold` = Bold text
- `text-blue-600` = Blue color
- `mb-4` = Margin (space) below the element

### Common Tailwind Classes Used in This Landing Page

#### Text Styling

| Class | Purpose | Example |
|-------|---------|---------|
| `text-sm` | Small text | Announcement bar |
| `text-lg` | Large text | Body text |
| `text-2xl` | Extra large text | Section headings |
| `text-3xl` | Even larger | Main headings |
| `font-bold` | Bold text | Titles |
| `font-semibold` | Semi-bold text | Subtitles |
| `font-medium` | Medium weight | Regular text |
| `text-gray-900` | Dark gray/black text | Main text |
| `text-gray-700` | Medium gray text | Secondary text |
| `text-gray-600` | Lighter gray text | Tertiary text |
| `text-white` | White text | On dark backgrounds |
| `text-blue-600` | Blue text | Links, accents |

#### Colors

The landing page uses a color system. Here are the main colors:

**Background Colors:**
- `bg-white` = White background
- `bg-gray-50` = Very light gray
- `bg-gray-900` = Very dark gray/black
- `bg-blue-600` = Blue (primary color)
- `bg-purple-600` = Purple
- `bg-green-600` = Green

**Text Colors:**
- `text-gray-900` = Dark text
- `text-blue-600` = Blue text
- `text-white` = White text

#### Spacing

| Class | Purpose | Size |
|-------|---------|------|
| `mb-4` | Margin bottom | Small space below |
| `mb-6` | Margin bottom | Medium space below |
| `mb-8` | Margin bottom | Large space below |
| `mt-4` | Margin top | Small space above |
| `px-4` | Padding horizontal | Horizontal padding |
| `py-4` | Padding vertical | Vertical padding |
| `p-8` | Padding all sides | All-around padding |

#### Layout

| Class | Purpose | Use |
|-------|---------|-----|
| `flex` | Flexbox layout | Arrange items horizontally |
| `grid` | Grid layout | Create columns |
| `grid-cols-1` | One column | Mobile view |
| `md:grid-cols-2` | Two columns on medium screens | Tablet and up |
| `lg:grid-cols-3` | Three columns on large screens | Desktop and up |
| `gap-8` | Space between grid items | Gap between columns |

#### Responsive Design

Tailwind uses prefixes for different screen sizes:

- **No prefix** = Mobile (default)
- **`sm:`** = Small screens (640px and up)
- **`md:`** = Medium screens (768px and up)
- **`lg:`** = Large screens (1024px and up)

**Example:**
```html
<div class="text-2xl md:text-4xl lg:text-5xl">
    Text size: 2xl on mobile, 4xl on tablets, 5xl on desktop
</div>
```

#### Rounded Corners

| Class | Purpose |
|-------|---------|
| `rounded-lg` | Slightly rounded corners |
| `rounded-xl` | More rounded corners |
| `rounded-2xl` | Very rounded corners |
| `rounded-full` | Completely circular |

#### Shadows

| Class | Effect |
|-------|--------|
| `shadow-md` | Medium shadow |
| `shadow-lg` | Large shadow |
| `hover:shadow-xl` | Extra large shadow on hover |

#### Transitions & Hover Effects

| Class | Purpose |
|-------|---------|
| `transition-all` | Smooth transition |
| `duration-300` | 300ms animation time |
| `hover:` | Applies on mouse hover |
| `hover:bg-blue-700` | Darker blue on hover |
| `hover:text-blue-600` | Blue text on hover |

### How to Modify Tailwind Classes

#### Example 1: Change Text Color

**Original:**
```html
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mb-4 tracking-tight">
    Powerful Features
</h2>
```

**Change text from dark gray to blue:**
```html
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-blue-600 mb-4 tracking-tight">
    Powerful Features
</h2>
```

**What changed:** `text-gray-900` → `text-blue-600`

---

#### Example 2: Change Button Color

**Original:**
```html
<a href="https://lpk.com" class="btn-primary bg-blue-600 hover:bg-blue-700 text-white px-8 py-4 rounded-lg font-semibold shadow-md hover:shadow-lg">
    Buy Now
</a>
```

**Change to green:**
```html
<a href="https://lpk.com" class="btn-primary bg-green-600 hover:bg-green-700 text-white px-8 py-4 rounded-lg font-semibold shadow-md hover:shadow-lg">
    Buy Now
</a>
```

**What changed:** 
- `bg-blue-600` → `bg-green-600` (button color)
- `hover:bg-blue-700` → `hover:bg-green-700` (hover color)

---

#### Example 3: Change Background Color

**Original:**
```html
<section id="features" class="py-16 md:py-24 bg-white">
```

**Change to light gray:**
```html
<section id="features" class="py-16 md:py-24 bg-gray-50">
```

**What changed:** `bg-white` → `bg-gray-50`

---

#### Example 4: Adjust Spacing

**Original:**
```html
<div class="mb-12 md:mb-16">
    Content here
</div>
```

**Increase bottom margin:**
```html
<div class="mb-16 md:mb-20">
    Content here
</div>
```

**What changed:** `mb-12` → `mb-16` and `md:mb-16` → `md:mb-20`

---

#### Example 5: Change Grid Columns

**Original (3 columns on desktop):**
```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
```

**Change to 2 columns on desktop:**
```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
```

**What changed:** `md:grid-cols-3` → `md:grid-cols-2`

---

### Responsive Design Best Practices

When modifying Tailwind classes, always consider mobile, tablet, and desktop views:

**Good Practice:**
```html
<h1 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl">
    Responsive Heading
</h1>
```

This means:
- Mobile: `text-2xl` (smaller on phones)
- Small screens: `text-3xl` (medium on small tablets)
- Medium screens: `text-4xl` (larger on tablets)
- Large screens: `text-5xl` (largest on desktop)

**How to Apply:**
1. Start with mobile-first classes (no prefix)
2. Add medium screen classes (`md:`)
3. Add large screen classes (`lg:`)
4. Always test on different screen sizes

---

## Managing Links

### Understanding Links in Your Landing Page

Your landing page contains several types of links:

1. **Navigation menu links** - Jump to sections
2. **Button links** - External URLs (Shop Now, Buy Now)
3. **Footer links** - To other pages and social media
4. **Internal anchor links** - Jump to sections on same page

### Navigation Menu Links

**Location:** Lines 101-107 (Desktop) and Lines 117-123 (Mobile)

**Current Links:**
```html
<a href="#home" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Home</a>
<a href="#features" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Features</a>
<a href="#benefits" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Benefits</a>
<a href="#about" class="nav-link text-gray-700 hover:text-blue-600 font-medium">About</a>
<a href="#testimonials" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Testimonials</a>
<a href="#faq" class="nav-link text-gray-700 hover:text-blue-600 font-medium">FAQ</a>
<a href="#contact" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Contact</a>
```

**Understanding the `href` Attribute:**
- `href="#home"` - Links to section with `id="home"`
- `#` symbol means "jump to a section on this page"
- The text after `#` must match a section ID exactly

**Sections in Your Page:**
- `#home` - Hero section (line 148)
- `#features` - Features section (line 174)
- `#benefits` - Benefits section (line 239)
- `#about` - About section (line 374)
- `#testimonials` - Testimonials section (line 439)
- `#faq` - FAQ section (line 538)
- `#contact` - Contact section (line 624)

**How to Add a New Navigation Link:**

1. **Add the section ID** to your new section:
```html
<section id="pricing" class="py-16 md:py-24 bg-white">
    <!-- Your pricing content here -->
</section>
```

2. **Add the link** to the navigation menu (lines 101-107):
```html
<a href="#pricing" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Pricing</a>
```

3. **Add it to mobile menu** too (lines 117-123):
```html
<a href="#pricing" class="text-gray-700 hover:text-blue-600 font-medium transition-colors duration-300">Pricing</a>
```

---

### External Links (Shop Now / Buy Now Buttons)

**Locations:**
- Hero section button: Line 162
- CTA section button: Line 350
- Header button: Line 113
- Mobile menu button: Line 127

**Current Link:**
```html
<a href="https://lpk.com" class="btn-primary bg-blue-600 hover:bg-blue-700 text-white px-8 py-4 rounded-lg font-semibold shadow-md hover:shadow-lg">
    Buy Now
</a>
```

**How to Update External Links:**

Replace `https://lpk.com` with your actual store URL:

```html
<a href="https://yourstore.com/products/led-lightbox" class="btn-primary bg-blue-600 hover:bg-blue-700 text-white px-8 py-4 rounded-lg font-semibold shadow-md hover:shadow-lg">
    Buy Now
</a>
```

**Important:** Include `https://` at the beginning of external URLs.

---

### Footer Links

**Location:** Lines 745-759, 768-778

**Quick Links Section (Lines 745-759):**
```html
<ul class="space-y-2">
    <li><a href="#home" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">Home</a></li>
    <li><a href="#features" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">Features</a></li>
    <li><a href="#benefits" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">Benefits</a></li>
    <li><a href="#about" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">About Us</a></li>
    <li><a href="#testimonials" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">Testimonials</a></li>
</ul>
```

These links should match your navigation menu links.

**Support Links Section (Lines 750-759):**
```html
<ul class="space-y-2">
    <li><a href="#faq" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">FAQ</a></li>
    <li><a href="#contact" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">Contact Us</a></li>
    <li><a href="privacy.html" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="terms.html" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">Terms of Service</a></li>
    <li><a href="blog.html" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">Blog</a></li>
</ul>
```

**Contact Info Links (Lines 768-778):**
```html
<li class="flex items-start">
    <i class="fas fa-envelope text-blue-500 mr-3 mt-1"></i>
    <a href="mailto:admin@lpk.com" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">admin@lpk.com</a>
</li>
<li class="flex items-start">
    <i class="fas fa-globe text-blue-500 mr-3 mt-1"></i>
    <a href="https://lpk.com" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">lpk.com</a>
</li>
```

**How to Update Email Link:**
```html
<a href="mailto:youremail@yourcompany.com" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">youremail@yourcompany.com</a>
```

**How to Update Website Link:**
```html
<a href="https://yourwebsite.com" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">yourwebsite.com</a>
```

---

### Social Media Links

**Location:** Lines 725-735

**Current Links:**
```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">
        <i class="fab fa-facebook-f text-xl"></i>
    </a>
    <a href="#" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">
        <i class="fab fa-twitter text-xl"></i>
    </a>
    <a href="#" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">
        <i class="fab fa-instagram text-xl"></i>
    </a>
    <a href="#" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">
        <i class="fab fa-youtube text-xl"></i>
    </a>
</div>
```

**How to Update Social Media Links:**

Replace `href="#"` with your actual social media URLs:

```html
<!-- Facebook -->
<a href="https://facebook.com/yourpage" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">
    <i class="fab fa-facebook-f text-xl"></i>
</a>

<!-- Twitter -->
<a href="https://twitter.com/yourprofile" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">
    <i class="fab fa-twitter text-xl"></i>
</a>

<!-- Instagram -->
<a href="https://instagram.com/yourprofile" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">
    <i class="fab fa-instagram text-xl"></i>
</a>

<!-- YouTube -->
<a href="https://youtube.com/@yourchannel" class="text-gray-400 hover:text-blue-500 transition-colors duration-300">
    <i class="fab fa-youtube text-xl"></i>
</a>
```

---

### Logo Link

**Location:** Lines 96-98

**Current:**
```html
<a href="#" class="text-2xl font-bold text-gray-900 hover:text-blue-600 transition-colors duration-300">
    <i class="fas fa-lightbulb text-blue-600 mr-2"></i>LPK
</a>
```

**Update to go to home section:**
```html
<a href="#home" class="text-2xl font-bold text-gray-900 hover:text-blue-600 transition-colors duration-300">
    <i class="fas fa-lightbulb text-blue-600 mr-2"></i>LPK
</a>
```

---

### Testing Your Links

After updating links:

1. **Save your file** (`Ctrl+S` or `Cmd+S`)
2. **Refresh your browser** (`F5` or `Cmd+R`)
3. **Click each link** to verify it works
4. **Check mobile view** - Use browser's responsive design mode (`F12`)

---

## Adding Privacy and Terms Pages

### Overview

Your landing page currently links to `privacy.html` and `terms.html`, but these files don't exist yet. This section shows you how to create them.

### Step 1: Create the Privacy Policy Page

**Create a new file named `privacy.html` in the same folder as `index.html`**

1. Open your text editor
2. Go to File → New File
3. Copy the following code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - LED Lightbox Kit">
    <meta name="author" content="LED Lightbox Kit">
    <title>Privacy Policy - LED Lightbox Kit</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900 font-sans">
    
    <!-- Header/Navigation -->
    <header class="sticky top-0 z-50 bg-white border-b border-gray-200 shadow-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Logo -->
                <div class="flex-shrink-0">
                    <a href="index.html" class="text-2xl font-bold text-gray-900 hover:text-blue-600 transition-colors duration-300">
                        <i class="fas fa-lightbulb text-blue-600 mr-2"></i>LPK
                    </a>
                </div>

                <!-- Desktop Navigation -->
                <nav class="hidden md:flex items-center space-x-8">
                    <a href="index.html#home" class="text-gray-700 hover:text-blue-600 font-medium">Home</a>
                    <a href="index.html#contact" class="text-gray-700 hover:text-blue-600 font-medium">Contact</a>
                </nav>

                <!-- Right Side Items -->
                <div class="hidden md:flex items-center space-x-4">
                    <a href="https://lpk.com" class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-2 rounded-lg font-semibold shadow-md hover:shadow-lg">
                        Buy Now
                    </a>
                </div>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <section class="py-16 md:py-24 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">Privacy Policy</h1>
            
            <div class="prose prose-lg text-gray-700 space-y-6">
                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">1. Introduction</h2>
                    <p>
                        LED Lightbox Kit ("we," "us," "our," or "Company") is committed to protecting your privacy. 
                        This Privacy Policy explains how we collect, use, disclose, and otherwise handle your information 
                        when you visit our website and use our services.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">2. Information We Collect</h2>
                    <p>
                        We may collect information about you in a variety of ways. The information we may collect on the 
                        site includes:
                    </p>
                    <ul class="list-disc list-inside space-y-2 mt-3">
                        <li>Name and email address</li>
                        <li>Phone number</li>
                        <li>Billing and shipping address</li>
                        <li>Payment information</li>
                        <li>Information about your browsing habits</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">3. How We Use Your Information</h2>
                    <p>
                        We use the information we collect in various ways, including to:
                    </p>
                    <ul class="list-disc list-inside space-y-2 mt-3">
                        <li>Process your transactions and send related information</li>
                        <li>Send marketing and promotional emails</li>
                        <li>Respond to your inquiries and provide customer support</li>
                        <li>Improve our website and services</li>
                        <li>Comply with legal obligations</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">4. Protection of Your Information</h2>
                    <p>
                        We implement a variety of security measures to maintain the safety of your personal information. 
                        Your personal information is contained behind secured networks and is only accessible by a limited 
                        number of persons who have special access rights to such systems.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">5. Disclosure of Your Information</h2>
                    <p>
                        We do not sell, trade, or otherwise transfer to outside parties your personally identifiable 
                        information unless we provide you with advance notice. This does not include website hosting partners 
                        and other parties who assist us in operating our website, conducting our business, or servicing you.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">6. Cookies</h2>
                    <p>
                        Our website may use "cookies" to enhance user experience. You can choose to have your computer warn 
                        you each time a cookie is being sent, or you can choose to turn off all cookies through your browser settings.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">7. Third-Party Links</h2>
                    <p>
                        Occasionally, at our discretion, we may include or offer third-party products or services on our website. 
                        These third-party sites have separate and independent privacy policies. We therefore have no responsibility 
                        or liability for the content and activities of these linked sites.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">8. Changes to This Privacy Policy</h2>
                    <p>
                        We may update this Privacy Policy at any time. When we do, we will revise the updated date at the bottom 
                        of this page and notify you via email if the changes are material.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">9. Contact Us</h2>
                    <p>
                        If you have questions or comments about this Privacy Policy, please contact us at:
                    </p>
                    <p class="mt-3">
                        <strong>Email:</strong> <a href="mailto:admin@lpk.com" class="text-blue-600 hover:text-blue-700">admin@lpk.com</a>
                    </p>
                </div>

                <div class="pt-6 border-t border-gray-300">
                    <p class="text-gray-600 text-sm">
                        Last updated: <span id="lastUpdated"></span>
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12 md:py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center">
                <p class="text-gray-400 text-sm">
                    &copy; <span id="year">2024</span> LED Lightbox Kit. All rights reserved.
                </p>
            </div>
        </div>
    </footer>

    <script>
        // Update year in footer
        document.getElementById('year').textContent = new Date().getFullYear();
        document.getElementById('lastUpdated').textContent = new Date().toLocaleDateString('en-US', { 
            year: 'numeric', 
            month: 'long', 
            day: 'numeric' 
        });
    </script>
</body>
</html>
```

4. Save this file as `privacy.html` in the same folder as `index.html`

---

### Step 2: Create the Terms of Service Page

**Create a new file named `terms.html` in the same folder as `index.html`**

1. Open your text editor
2. Go to File → New File
3. Copy the following code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - LED Lightbox Kit">
    <meta name="author" content="LED Lightbox Kit">
    <title>Terms of Service - LED Lightbox Kit</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900 font-sans">
    
    <!-- Header/Navigation -->
    <header class="sticky top-0 z-50 bg-white border-b border-gray-200 shadow-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Logo -->
                <div class="flex-shrink-0">
                    <a href="index.html" class="text-2xl font-bold text-gray-900 hover:text-blue-600 transition-colors duration-300">
                        <i class="fas fa-lightbulb text-blue-600 mr-2"></i>LPK
                    </a>
                </div>

                <!-- Desktop Navigation -->
                <nav class="hidden md:flex items-center space-x-8">
                    <a href="index.html#home" class="text-gray-700 hover:text-blue-600 font-medium">Home</a>
                    <a href="index.html#contact" class="text-gray-700 hover:text-blue-600 font-medium">Contact</a>
                </nav>

                <!-- Right Side Items -->
                <div class="hidden md:flex items-center space-x-4">
                    <a href="https://lpk.com" class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-2 rounded-lg font-semibold shadow-md hover:shadow-lg">
                        Buy Now
                    </a>
                </div>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <section class="py-16 md:py-24 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">Terms of Service</h1>
            
            <div class="prose prose-lg text-gray-700 space-y-6">
                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">1. Agreement to Terms</h2>
                    <p>
                        By accessing and using this website, you accept and agree to be bound by the terms and provision 
                        of this agreement. If you do not agree to abide by the above, please do not use this service.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">2. Use License</h2>
                    <p>
                        Permission is granted to temporarily download one copy of the materials (information or software) 
                        on LED Lightbox Kit's website for personal, non-commercial transitory viewing only. This is the grant 
                        of a license, not a transfer of title, and under this license you may not:
                    </p>
                    <ul class="list-disc list-inside space-y-2 mt-3">
                        <li>Modify or copy the materials</li>
                        <li>Use the materials for any commercial purpose or for any public display</li>
                        <li>Attempt to decompile or reverse engineer any software contained on the website</li>
                        <li>Remove any copyright or other proprietary notations from the materials</li>
                        <li>Transfer the materials to another person or "mirror" the materials on any other server</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">3. Disclaimer</h2>
                    <p>
                        The materials on LED Lightbox Kit's website are provided on an 'as is' basis. LED Lightbox Kit 
                        makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties 
                        including, without limitation, implied warranties or conditions of merchantability, fitness for 
                        a particular purpose, or non-infringement of intellectual property or other violation of rights.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">4. Limitations</h2>
                    <p>
                        In no event shall LED Lightbox Kit or its suppliers be liable for any damages (including, without 
                        limitation, damages for loss of data or profit, or due to business interruption) arising out of the 
                        use or inability to use the materials on LED Lightbox Kit's website, even if LED Lightbox Kit or an 
                        authorized representative has been notified orally or in writing of the possibility of such damage.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">5. Accuracy of Materials</h2>
                    <p>
                        The materials appearing on LED Lightbox Kit's website could include technical, typographical, or 
                        photographic errors. LED Lightbox Kit does not warrant that any of the materials on its website are 
                        accurate, complete, or current. LED Lightbox Kit may make changes to the materials contained on its 
                        website at any time without notice.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">6. Links</h2>
                    <p>
                        LED Lightbox Kit has not reviewed all of the sites linked to its website and is not responsible for 
                        the contents of any such linked site. The inclusion of any link does not imply endorsement by LED 
                        Lightbox Kit of the site. Use of any such linked website is at the user's own risk.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">7. Modifications</h2>
                    <p>
                        LED Lightbox Kit may revise these terms of service for its website at any time without notice. 
                        By using this website, you are agreeing to be bound by the then current version of these terms of service.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">8. Governing Law</h2>
                    <p>
                        These terms and conditions are governed by and construed in accordance with the laws of the jurisdiction 
                        in which LED Lightbox Kit is located, and you irrevocably submit to the exclusive jurisdiction of the 
                        courts in that location.
                    </p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">9. Contact Us</h2>
                    <p>
                        If you have any questions about these Terms of Service, please contact us at:
                    </p>
                    <p class="mt-3">
                        <strong>Email:</strong> <a href="mailto:admin@lpk.com" class="text-blue-600 hover:text-blue-700">admin@lpk.com</a>
                    </p>
                </div>

                <div class="pt-6 border-t border-gray-300">
                    <p class="text-gray-600 text-sm">
                        Last updated: <span id="lastUpdated"></span>
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12 md:py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center">
                <p class="text-gray-400 text-sm">
                    &copy; <span id="year">2024</span> LED Lightbox Kit. All rights reserved.
                </p>
            </div>
        </div>
    </footer>

    <script>
        // Update year in footer
        document.getElementById('year').textContent = new Date().getFullYear();
        document.getElementById('lastUpdated').textContent = new Date().toLocaleDateString('en-US', { 
            year: 'numeric', 
            month: 'long', 
            day: 'numeric' 
        });
    </script>
</body>
</html>
```

4. Save this file as `terms.html` in the same folder as `index.html`

---

### Step 3: Create a Blog Page (Optional)

Your footer also references `blog.html`. Here's a simple template:

**Create a new file named `blog.html`:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Blog - LED Lightbox Kit">
    <meta name="author" content="LED Lightbox Kit">
    <title>Blog - LED Lightbox Kit</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body class="bg-white text-gray-900 font-sans">
    
    <!-- Header/Navigation -->
    <header class="sticky top-0 z-50 bg-white border-b border-gray-200 shadow-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Logo -->
                <div class="flex-shrink-0">
                    <a href="index.html" class="text-2xl font-bold text-gray-900 hover:text-blue-600 transition-colors duration-300">
                        <i class="fas fa-lightbulb text-blue-600 mr-2"></i>LPK
                    </a>
                </div>

                <!-- Desktop Navigation -->
                <nav class="hidden md:flex items-center space-x-8">
                    <a href="index.html#home" class="text-gray-700 hover:text-blue-600 font-medium">Home</a>
                    <a href="index.html#contact" class="text-gray-700 hover:text-blue-600 font-medium">Contact</a>
                </nav>

                <!-- Right Side Items -->
                <div class="hidden md:flex items-center space-x-4">
                    <a href="https://lpk.com" class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-2 rounded-lg font-semibold shadow-md hover:shadow-lg">
                        Buy Now
                    </a>
                </div>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <section class="py-16 md:py-24 bg-white">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12 md:mb-16">
                <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-4">Blog</h1>
                <p class="text-lg md:text-xl text-gray-600">
                    Tips, tutorials, and insights for professional photographers
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Blog Post 1 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-md hover:shadow-lg transition-shadow duration-300 border border-gray-200">
                    <div class="bg-gradient-to-r from-blue-500 to-blue-600 h-48"></div>
                    <div class="p-6">
                        <p class="text-sm text-gray-600 mb-2">Posted on January 15, 2024</p>
                        <h3 class="text-xl font-bold text-gray-900 mb-3">Getting Started with LED Lighting</h3>
                        <p class="text-gray-700 mb-4">
                            Learn the basics of LED lighting and how to get professional results with your first setup.
                        </p>
                        <a href="#" class="text-blue-600 hover:text-blue-700 font-semibold">Read More →</a>
                    </div>
                </div>

                <!-- Blog Post 2 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-md hover:shadow-lg transition-shadow duration-300 border border-gray-200">
                    <div class="bg-gradient-to-r from-purple-500 to-purple-600 h-48"></div>
                    <div class="p-6">
                        <p class="text-sm text-gray-600 mb-2">Posted on January 10, 2024</p>
                        <h3 class="text-xl font-bold text-gray-900 mb-3">Color Temperature Guide</h3>
                        <p class="text-gray-700 mb-4">
                            Understanding color temperature and how to use it to enhance your photography.
                        </p>
                        <a href="#" class="text-blue-600 hover:text-blue-700 font-semibold">Read More →</a>
                    </div>
                </div>

                <!-- Blog Post 3 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-md hover:shadow-lg transition-shadow duration-300 border border-gray-200">
                    <div class="bg-gradient-to-r from-green-500 to-green-600 h-48"></div>
                    <div class="p-6">
                        <p class="text-sm text-gray-600 mb-2">Posted on January 5, 2024</p>
                        <h3 class="text-xl font-bold text-gray-900 mb-3">Energy-Efficient Studio Setup</h3>
                        <p class="text-gray-700 mb-4">
                            How to save money while maintaining professional-quality lighting in your studio.
                        </p>
                        <a href="#" class="text-blue-600 hover:text-blue-700 font-semibold">Read More →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12 md:py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center">
                <p class="text-gray-400 text-sm">
                    &copy; <span id="year">2024</span> LED Lightbox Kit. All rights reserved.
                </p>
            </div>
        </div>
    </footer>

    <script>
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>
```

Save this as `blog.html` in the same folder.

---

### Step 4: Verify All Links Work

**Your file structure should now look like:**
```
your-project-folder/
├── index.html
├── privacy.html
├── terms.html
└── blog.html
```

**Test all links:**
1. Open `index.html` in your browser
2. Click on "Privacy Policy" link in footer - should go to `privacy.html`
3. Click on "Terms of Service" link in footer - should go to `terms.html`
4. Click on "Blog" link in footer - should go to `blog.html`
5. On each policy/blog page, click the logo to return to `index.html`

---

### Step 5: Customize Policy Content

The template pages provided are basic examples. You should customize them with:

1. **Your actual company information**
2. **Your specific policies**
3. **Your contact details**
4. **Your business practices**

**Key sections to customize:**

In `privacy.html`:
- Change "admin@lpk.com" to your email
- Update privacy practices to match your business
- Add any specific data collection methods you use

In `terms.html`:
- Change "admin@lpk.com" to your email
- Update terms to match your business model
- Add warranty and return information
- Include shipping and payment terms

In `blog.html`:
- Replace placeholder blog posts with real content
- Update dates and titles
- Add actual blog post links

---

## Common Customizations

### Changing the Primary Color (Blue to Another Color)

The landing page uses blue (`blue-600`) as the primary color. To change it throughout:

**Find all instances of:**
- `bg-blue-600`
- `text-blue-600`
- `hover:bg-blue-700`
- `hover:text-blue-600`
- `border-blue-200`

**Replace with your color:**
- `bg-blue-600` → `bg-green-600` (for green)
- `bg-blue-600` → `bg-red-600` (for red)
- `bg-blue-600` → `bg-purple-600` (for purple)

**Tailwind Color Options:**
- Red: `red-600`
- Orange: `orange-600`
- Yellow: `yellow-600`
- Green: `green-600`
- Teal: `teal-600`
- Purple: `purple-600`
- Pink: `pink-600`

---

### Changing Hero Background Image

**Location:** Line 151

**Current:**
```html
<img src="https://images.unsplash.com/photo-1504093376055-b3094b674dcb?w=1600&h=900&fit=crop&q=80" alt="LED Lightbox Kit Hero">
```

**How to Change:**
1. Find a royalty-free image on Unsplash.com or Pexels.com
2. Get the image URL
3. Replace the entire URL in `src="..."`

**Example:**
```html
<img src="https://images.unsplash.com/photo-1611532736597-de2d4265fba3?w=1600&h=900&fit=crop&q=80" alt="Photography Studio">
```

---

### Changing Feature Card Icons

**Location:** Lines 189, 204, 219

Feature icons use Font Awesome. Find the icon class and replace:

**Current icons:**
- `fas fa-camera` (Professional Photography)
- `fas fa-briefcase` (Portable Setup)
- `fas fa-leaf` (Energy Efficient)

**Popular alternatives:**
- `fas fa-star` (star)
- `fas fa-heart` (heart)
- `fas fa-zap` (lightning bolt)
- `fas fa-rocket` (rocket)
- `fas fa-shield-alt` (shield)
- `fas fa-check` (checkmark)

**How to change:**
```html
<!-- Original -->
<i class="fas fa-camera text-white text-2xl"></i>

<!-- Changed to rocket -->
<i class="fas fa-rocket text-white text-2xl"></i>
```

**Find more icons at:** fontawesome.com/icons

---

### Adding a New Section

**Template for adding a new section:**

```html
<!-- New Section -->
<section id="newsection" class="py-16 md:py-24 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-12 md:mb-16">
            <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mb-4 tracking-tight">
                Section Title
            </h2>
            <p class="text-lg md:text-xl text-gray-600 max-w-2xl mx-auto leading-relaxed">
                Section subtitle or description
            </p>
        </div>

        <!-- Your content here -->

    </div>
</section>
```

**Don't forget to:**
1. Add the section ID (e.g., `id="newsection"`)
2. Add it to the navigation menu with matching href (e.g., `href="#newsection"`)
3. Add it to the footer quick links

---

### Changing Button Text

**Locations of buttons:**
- Hero section: Lines 162-165
- CTA section: Lines 350-357
- Header: Line 113
- Mobile menu: Line 127

**How to change:**
```html
<!-- Original -->
<a href="https://lpk.com" class="btn-primary bg-blue-600 hover:bg-blue-700 text-white px-8 py-4 rounded-lg font-semibold shadow-md hover:shadow-lg">
    Buy Now
</a>

<!-- Changed -->
<a href="https://lpk.com" class="btn-primary bg-blue-600 hover:bg-blue-700 text-white px-8 py-4 rounded-lg font-semibold shadow-md hover:shadow-lg">
    Get Started Today
</a>
```

---

### Changing Feature Card Colors

Each feature card has a different color. To change them:

**Feature 1 (Professional Photography):**
- Line 183: Change `from-blue-50 to-blue-100` to different gradient
- Line 184: Change `border-blue-200` to match
- Line 189: Change `bg-blue-600` to match

**Feature 2 (Portable Setup):**
- Line 198: Change `from-purple-50 to-purple-100`
- Line 199: Change `border-purple-200`
- Line 204: Change `bg-purple-600`

**Feature 3 (Energy Efficient):**
- Line 213: Change `from-green-50 to-green-100`
- Line 214: Change `border-green-200`
- Line 219: Change `bg-green-600`

**Example - Change Feature 1 to orange:**
```html
<div class="feature-card bg-gradient-to-br from-orange-50 to-orange-100 p-8 rounded-2xl border border-orange-200 hover:shadow-xl">
    <div class="mb-6 flex items-center justify-center w-16 h-16 bg-orange-600 rounded-full">
        <i class="fas fa-camera text-white text-2xl"></i>
    </div>
```

---

## Troubleshooting

### Problem: Links Not Working

**Symptom:** Clicking a link doesn't navigate anywhere

**Solutions:**

1. **Check the href attribute:**
   - Internal links should have `href="#sectionname"`
   - External links should have `href="https://website.com"`
   - Missing `https://` on external links breaks them

2. **Verify section IDs exist:**
   - If linking to `#features`, make sure there's a `<section id="features">` somewhere
   - IDs are case-sensitive: `#Features` won't match `id="features"`

3. **Check for typos:**
   - `href="#feautres"` won't work (typo in "features")
   - Compare the href with the actual id

**Fix example:**
```html
<!-- Wrong -->
<a href="#feature">Features</a>
<section id="features">...</section>

<!-- Correct -->
<a href="#features">Features</a>
<section id="features">...</section>
```

---

### Problem: Text Changes Don't Appear

**Symptom:** You edited text but the website still shows old text

**Solutions:**

1. **Save the file:**
   - Use `Ctrl+S` (or `Cmd+S` on Mac)
   - Make sure the file is saved (check title bar - should not have asterisk)

2. **Refresh the browser:**
   - Press `F5` or `Ctrl+R` (or `Cmd+R` on Mac)
   - Or click the refresh button in your browser

3. **Clear browser cache:**
   - Press `Ctrl+Shift+Delete` (or `Cmd+Shift+Delete` on Mac)
   - Select "Cached images and files"
   - Click "Clear"

4. **Check you edited the right file:**
   - Make sure you're editing `index.html` not a copy
   - Check the file path in your text editor

---

### Problem: Styling Looks Broken

**Symptom:** Colors, spacing, or layout looks wrong

**Solutions:**

1. **Check Tailwind CDN link:**
   - Line 13 should have: `<script src="https://cdn.tailwindcss.com"></script>`
   - If this is missing or broken, no styling will work

2. **Check for typos in class names:**
   - `text-2x1` (with number 1) won't work
   - Should be `text-2xl` (with lowercase L)
   - Tailwind classes are case-sensitive

3. **Verify you didn't break HTML structure:**
   - Every opening tag needs a closing tag
   - Example: `<div>` needs `</div>`
   - Missing closing tags break styling

4. **Check for missing quotes:**
   - `class="text-2xl"` (correct)
   - `class=text-2xl` (wrong - missing quotes)

---

### Problem: Mobile Menu Not Working

**Symptom:** Menu button doesn't open/close menu on mobile

**Solutions:**

1. **Check JavaScript is present:**
   - Lines 848-875 contain the menu toggle code
   - Don't delete this code

2. **Verify HTML structure:**
   - `.mobile-menu-button` must exist (line 131)
   - `.mobile-menu` must exist (line 134)
   - They must be spelled exactly the same

3. **Test on actual mobile:**
   - Use browser's responsive design mode (F12)
   - Resize to mobile width (less than 768px)
   - Menu should appear on screens smaller than 768px

---

### Problem: FAQ Accordion Not Working

**Symptom:** Clicking FAQ questions doesn't expand answers

**Solutions:**

1. **Check JavaScript is present:**
   - Lines 832-845 contain the FAQ toggle code
   - Don't delete this code

2. **Verify class names:**
   - `.faq-toggle` buttons must exist
   - `.faq-item` containers must exist
   - `.faq-content` divs must exist

3. **Check CSS transitions:**
   - Lines 35-44 contain FAQ styling
   - Don't delete this CSS

---

### Problem: Images Not Showing

**Symptom:** Image placeholders appear instead of actual images

**Solutions:**

1. **Check image URLs:**
   - External images use full URLs starting with `https://`
   - Check the URL is correct and accessible

2. **Test the image URL:**
   - Copy the image URL into your browser address bar
   - If it doesn't load, the URL is broken

3. **Use a different image source:**
   - Unsplash.com (free high-quality images)
   - Pexels.com (free stock photos)
   - Pixabay.com (free images)

**Example - Replace image:**
```html
<!-- Old -->
<img src="https://images.unsplash.com/old-image-id" alt="Description">

<!-- New -->
<img src="https://images.unsplash.com/photo-1234567890123-abcdefghijk?w=800&h=600&fit=crop&q=80" alt="Description">
```

---

### Problem: Email Links Not Working

**Symptom:** Clicking email link doesn't open email client

**Solution:**

Make sure email links use `mailto:` prefix:

```html
<!-- Wrong -->
<a href="admin@lpk.com">Email us</a>

<!-- Correct -->
<a href="mailto:admin@lpk.com">Email us</a>
```

---

### Problem: Responsive Design Issues

**Symptom:** Website doesn't look good on mobile or tablet

**Solutions:**

1. **Test on multiple devices:**
   - Use browser's responsive design mode (F12)
   - Test at: 375px (mobile), 768px (tablet), 1024px (desktop)

2. **Check responsive classes:**
   - Mobile-first approach: no prefix for mobile
   - `md:` for tablets and up (768px+)
   - `lg:` for desktop and up (1024px+)

3. **Common responsive issues:**
   - Text too small: increase `text-lg` to `text-xl`
   - Columns not stacking: change `grid-cols-3` to `md:grid-cols-3`
   - Padding too large: reduce `p-8` to `p-4`

---

### Problem: Footer Links Point to Wrong Pages

**Symptom:** Footer links don't work or go to wrong pages

**Solutions:**

1. **Verify file names:**
   - Files should be: `index.html`, `privacy.html`, `terms.html`, `blog.html`
   - All lowercase, no spaces

2. **Check file locations:**
   - All files should be in the same folder
   - Don't put them in subfolders

3. **Verify links in footer:**
   - `href="privacy.html"` (correct)
   - `href="/privacy.html"` (wrong - slash means root folder)
   - `href="../privacy.html"` (wrong - goes up a folder)

---

### Problem: Form Not Submitting

**Symptom:** Contact form doesn't send messages

**Note:** The contact form in this template is a front-end only. To make it actually send emails, you need:

1. **Backend service** (like Formspree, Netlify Forms, or EmailJS)
2. **Form action attribute:**

```html
<!-- Add this to the form tag -->
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="space-y-6">
    <!-- form fields -->
</form>
```

**To set up Formspree (free):**
1. Go to formspree.io
2. Sign up for free account
3. Create a new form
4. Get your form ID
5. Update the form action in your HTML

---

## Best Practices for Maintenance

### Regular Updates

1. **Update links quarterly:**
   - Check all external links work
   - Update social media URLs if changed
   - Verify email addresses are current

2. **Refresh images annually:**
   - Replace outdated product images
   - Update testimonial photos
   - Refresh hero background

3. **Review content:**
   - Update statistics and numbers
   - Refresh testimonials
   - Update pricing or features

### Backup Your Files

1. **Keep backups:**
   - Save copies of your HTML files
   - Use version control (Git) if possible
   - Backup before major changes

2. **Test changes locally:**
   - Make changes on a copy first
   - Test thoroughly before publishing
   - Keep original as fallback

### Security

1. **Protect sensitive information:**
   - Don't put passwords in HTML
   - Use environment variables for API keys
   - Keep admin emails private

2. **Update external resources:**
   - Keep Tailwind CSS updated
   - Update Font Awesome if needed
   - Monitor for security updates

---

## Additional Resources

### Learning Resources

- **Tailwind CSS Documentation:** tailwindcss.com/docs
- **Font Awesome Icons:** fontawesome.com/icons
- **HTML Guide:** developer.mozilla.org/en-US/docs/Web/HTML
- **CSS Guide:** developer.mozilla.org/en-US/docs/Web/CSS

### Free Tools

- **Image Hosting:** Unsplash.com, Pexels.com, Pixabay.com
- **Color Picker:** coolors.co
- **Responsive Tester:** responsively.app
- **Code Editor:** VS Code (free)

### Support

- **Browser DevTools:** Press F12 to inspect elements
- **Console Errors:** Check browser console for errors
- **Stack Overflow:** Ask questions on stackoverflow.com

---

## Summary

You now have a complete guide to maintaining and customizing your LED Lightbox Kit landing page. Here's what you've learned:

✅ How to update text content in every section
✅ How to modify Tailwind CSS classes for styling
✅ How to manage and fix links
✅ How to create and link Privacy, Terms, and Blog pages
✅ How to make common customizations
✅ How to troubleshoot common problems

**Next Steps:**

1. Create `privacy.html`, `terms.html`, and `blog.html` files
2. Customize content for your business
3. Update all links to your actual URLs
4. Test everything on mobile, tablet, and desktop
5. Publish your updated website

Good luck with your landing page! 🚀