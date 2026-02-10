CSSCamp Documentation 🏕️
One CSS file. Everything included. Zero configuration.

Table of Contents
Installation

Colors

Spacing

Layout

Typography

Borders

Effects

Shapes

Components

Utilities

Examples

Installation
CDN
html
<!-- Development -->
<link rel="stylesheet" 
      href="https://cdn.jsdelivr.net/gh/yasin2343jaberynsar/CSSCamp@main/styles/csscamp.css">

<!-- Production -->
<link rel="stylesheet" 
      href="https://cdn.jsdelivr.net/gh/yasin2343jaberynsar/CSSCamp@main/styles/csscamp.min.css">
Download
csscamp.css (Unminified)

csscamp.min.css (Minified)

Colors
Background Colors
html
<div class="bg-primary">Blue</div>
<div class="bg-secondary">Gray</div>
<div class="bg-win">Green</div>
<div class="bg-lose">Red</div>
<div class="bg-info">Light Blue</div>
<div class="bg-yel">Yellow</div>
<div class="bg-solid">Orange</div>
<div class="bg-neon">Purple (#b01dce)</div>
<div class="bg-light">Light Gray</div>
<div class="bg-dark">Dark Gray</div>
Text Colors
html
<p class="text-primary">Blue text</p>
<p class="text-win">Green text</p>
<p class="text-neon">Purple text</p>
<p class="text-light">Light text</p>
<p class="text-dark">Dark text</p>
Available: .text-primary, .text-secondary, .text-win, .text-lose, .text-light, .text-dark, .text-info, .text-yel, .text-solid, .text-neon

Hover Colors
html
<button class="bg-primary bg-win-hover">Hover changes to green</button>
<a href="#" class="text-dark text-primary-h">Hover changes to blue</a>
Pattern: .bg-{color}-hover, .text-{color}-h

Spacing
Margin
html
<div class="m-5">5px margin all sides</div>
<div class="mt-10">10px top margin</div>
<div class="mb-10">10px bottom margin</div>
<div class="ml-10">10px left margin</div>
<div class="mr-10">10px right margin</div>
Padding
html
<div class="p-5">5px padding all sides</div>
<div class="pt-10">10px top padding</div>
<div class="pb-10">10px bottom padding</div>
<div class="pl-10">10px left padding</div>
<div class="pr-10">10px right padding</div>
Available Sizes
2, 3, 4, 5, 6, 7, 8, 9, 10, 15 pixels

Maximum: 15px (no 20, 25, etc.)

Missing: 11, 12, 13, 14

Pattern: .{m|p}{t|r|b|l}-{size}

Layout
Display
html
<div class="d-block">block</div>
<div class="d-flex">flex</div>
<div class="d-grid">grid</div>
<div class="d-inline">inline</div>
<div class="d-inline-block">inline-block</div>
<div class="d-inline-flex">inline-flex</div>
<div class="d-none">none</div>
Alias: .dead = .d-none

Flexbox
html
<!-- Container -->
<div class="d-flex">
  <div>Item</div>
  <div>Item</div>
</div>

<!-- Direction -->
<div class="d-flex flex-direction-row">Row</div>
<div class="d-flex flex-direction-col">Column</div>

<!-- Justify Content -->
<div class="d-flex justify-content-center">Center</div>
<div class="d-flex justify-content-flex-st">Flex start</div>
<div class="d-flex justify-content-flex-end">Flex end</div>
<div class="d-flex justify-content-space-between">Space between</div>

<!-- Align Items -->
<div class="d-flex align-items-center">Center</div>
<div class="d-flex align-items-flex-start">Flex start</div>
<div class="d-flex align-items-flex-end">Flex end</div>
Position
html
<div class="pos-relative">relative</div>
<div class="pos-absolute">absolute</div>
<div class="pos-fixed">fixed</div>
<div class="pos-sticky">sticky</div>
<div class="pos-static">static</div>
Centering
html
<div class="center">Center both</div>
<div class="center-hor">Center horizontal</div>
<div class="center-ver">Center vertical</div>
Note: Uses position: absolute

Z-index
html
<div class="z-index-0">0</div>
<div class="z-index-5">5</div>
<div class="z-index-10">10</div>
Available: 0 through 10

Typography
Font Sizes
html
<p class="font-size-10">10px</p>
<p class="font-size-16">16px</p>
<p class="font-size-20">20px</p>
<p class="font-size-30">30px</p>
<p class="font-size-40">40px</p>
Available: 10, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40

Text Decoration
html
<a class="txt-dec-none">No underline</a>
<span class="txt-dec-unline">Underline</span>
Direction
html
<div class="rtl">Right to left</div>
<div class="ltr">Left to right</div>
Borders
Border Radius
html
<div class="rounded-2">2px radius</div>
<div class="rounded-5">5px radius</div>
<div class="rounded-10">10px radius</div>
<div class="rounded-15">15px radius</div>
<div class="rounded-circle">Circle</div>
Available: 2, 3, 4, 5, 6, 7, 8, 9, 10, 15, circle
Missing: 11, 12, 13, 14

Alias: .badge = .rounded-7

Borders
html
<div class="border-all-1-primary">1px blue all sides</div>
<div class="border-top-2-win">2px green top</div>
<div class="border-bottom-3-dark">3px dark bottom</div>
<div class="border-left-4-neon">4px purple left</div>
<div class="border-right-5-solid">5px orange right</div>
Pattern: .border-{side}-{thickness}-{color}
Thickness: 1 to 10 pixels
Sides: all, top, bottom, left, right
Colors: All 10 colors

Effects
Opacity
html
<div class="op-0">0%</div>
<div class="op-05">50%</div>
<div class="op-1">100%</div>
Available: 0, 01 (10%), 02 (20%), 03, 04, 05, 06, 07, 08, 09, 1 (100%)

Blur
html
<div class="blur-5">5px backdrop blur</div>
<div class="full-blur-5">5px element blur</div>
Available: 1 to 16 pixels
Pattern: .blur-{1-16}, .full-blur-{1-16}

Glass Effect
html
<div class="royal-color-box">Glass box</div>
<div class="royal-color-box-in">Inset glass</div>
Transitions
html
<div class="trans-all-ease-03">0.3s ease</div>
<div class="trans-all-easein-05">0.5s ease-in</div>
<div class="trans-all-easeout-1">1s ease-out</div>
Pattern: .trans-all-{easing}-{duration}
Easing: ease, easein, easeout, easeio, lin
Duration: 01 (0.1s) to 1 (1s)

Animations
html
<div class="float">Floating</div>
<div class="glow-sm">Small glow</div>
<div class="glow-lg">Large glow</div>
<div class="breath-sm">Small breath</div>
<div class="breath-lg">Large breath</div>
<div class="floating-element-3">Floats every 3s</div>
Floating: .floating-element-{1-6} (1-6 seconds)

Shapes
Egg
html
<div class="egg">Medium</div>
<div class="egg-sm">Small</div>
<div class="egg-lg">Large</div>
Heart
html
<div class="heart">Heart</div>
Triangle
html
<div class="triangle">Red triangle</div>
<div class="triangle-primary">Blue</div>
<div class="triangle-win">Green</div>
<div class="triangle-neon">Purple</div>
Available: .triangle-{color} for all 10 colors

Components
Buttons
html
<button class="btn">Default button</button>
<button class="btn-bt">Alternative button</button>
Forms
html
<input class="form-control" placeholder="Input">
<textarea class="form-control"></textarea>
Progress Bars
html
<div class="progressbar-primary-50">50% blue</div>
<div class="progressbar-win-75">75% green</div>
<div class="progressbar-neon-25">25% purple</div>
Pattern: .progressbar-{color}-{percentage}
Percentage: 5 to 100 in steps of 5 (5, 10, 15, ..., 95, 100)
No 0%

Vertical: Rotate 90°

html
<div class="progressbar-primary-50 rotate-90"></div>
Tables
html
<table class="table">
  <tr><td>Data</td></tr>
</table>
Striped: .table-striped-p, .table-striped-l, .table-striped-d, .table-striped-da, .table-striped-s, .table-striped-so, .table-striped-in, .table-striped-y, .table-striped-sec

Utilities
Width & Height
html
<div class="w-50">50% width</div>
<div class="h-75">75% height</div>
<div class="w-100">100% width</div>
<div class="h-100">100% height</div>
Available: 0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65, 70, 75, 80, 85, 90, 95, 100

Rotation
html
<div class="rotate-5">5°</div>
<div class="rotate-45">45°</div>
<div class="rotate-90">90°</div>
<div class="rotate-180">180°</div>
Available:

5° to 120° in 5° steps

130° to 200° in 10° steps

Cursor
html
<div class="pc">Pointer cursor</div>
Overflow
html
<div class="overflow-hidden">Hidden</div>
<div class="overflow-scroll">Scroll</div>
Disabled
html
<button class="disabled">Can't click</button>
Examples
Alert Box
html
<div class="bg-win text-light p-10 rounded-5">
  Success message
</div>

<div class="bg-lose text-light p-10 rounded-5">
  Error message
</div>
Card
html
<div class="bg-light rounded-10 p-15">
  <h3 class="text-primary">Title</h3>
  <p class="text-dark">Content</p>
  <button class="btn bg-win text-light">Button</button>
</div>
Navbar
html
<nav class="bg-dark p-10 d-flex justify-content-space-between">
  <div class="text-primary">Logo</div>
  <div>
    <a href="#" class="text-light txt-dec-none ml-10">Home</a>
    <a href="#" class="text-light txt-dec-none ml-10">About</a>
  </div>
</nav>
Note: .ml-10 is max (no ml-20)

Browser Support
Chrome 49+

Firefox 52+

Safari 10.1+

Edge 16+

MIT

CSSCamp v1.0 • One file, everything included.
