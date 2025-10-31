# TV Test Pattern

A classic television test pattern implementation using HTML, CSS, and JavaScript. This project recreates a traditional TV test pattern used for calibrating displays, testing signal quality, and displaying technical information.

## Features

- **Classic Test Pattern Elements**
  - Checkered border with black and white squares
  - Color bars (SMPTE/EIA standard: Yellow, Cyan, Green, Magenta, Red, Blue)
  - Grayscale gradients (10 shades from black to white)
  - Vertical and horizontal test bars
  - Fine line patterns for detail testing

- **Interactive Elements**
  - Digital timers (HH:MM and DD-MM-YY formats)
  - Blinking colon animation on the first timer
  - Social media icons (Facebook, Instagram, X/Twitter)
  - Contact information display

- **Corner Indicators**
  - Four corner circles with aspect ratio indicators
  - Grid patterns for testing alignment
  - Different color schemes (white, blue, yellow backgrounds)

- **Responsive Design**
  - Responsive layout that adapts to different screen sizes
  - Mobile-friendly adjustments for smaller displays

## File Structure

```
tv-test-patern/
├── index.html      # Main HTML structure
├── styles.css      # All styling and layout
├── script.js       # JavaScript for timers and interactivity
└── README.md       # This file
```

## Getting Started

1. **Clone or download** the project files
2. **Open** `index.html` in a web browser
3. The test pattern will display automatically

No build process or dependencies required - it's pure HTML, CSS, and JavaScript!

## Project Structure

### HTML (`index.html`)

The HTML is organized into several main sections:
- **Border**: Checkered border with white bars at top and bottom
- **Central Circle**: Main test pattern area containing:
  - Top grayscale bars
  - Color bars with "COMING SOON" overlay
  - Timer display
  - Square grid patterns
  - Center black bar
  - Vertical grayscale gradient
  - Contact section with social icons
  - Fine lines pattern
  - Bottom color bars
- **Corner Circles**: Four corner indicators

### CSS (`styles.css`)

The stylesheet is organized into logical sections:
- Base styles and reset
- Border and background patterns
- Central circle layout
- Color bars styling
- Timer and center bar positioning
- Square grids
- Grayscale gradients
- Contact section
- Corner circles
- Responsive media queries

### JavaScript (`script.js`)

Handles:
- Timer functionality (updates time and date)
- Any dynamic animations or interactions

## Customization

### Changing Colors

Edit the color values in `styles.css`:

```css
/* Example: Change yellow bar color */
.color-bar.yellow {
    background: #your-color-here;
}
```

### Modifying Text

Update the text content in `index.html`:

```html
<!-- Change standby text -->
<div class="standby-text">YOUR TEXT HERE</div>

<!-- Change contact text -->
<div class="no-signal-text">YOUR CONTACT TEXT</div>
```

### Adjusting Social Media Links

Update the `href` attributes in `index.html`:

```html
<a href="YOUR_FACEBOOK_URL" class="social-icon" aria-label="Facebook">
```

### Modifying Timer Format

The timers are updated by `script.js`. Modify the JavaScript to change display formats or update intervals.

## Browser Compatibility

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile browsers (iOS Safari, Chrome Mobile)
- Responsive design tested on various screen sizes

## Color Standards

The color bars follow the **SMPTE/EIA standard**:
- Yellow: `#ffff00`
- Cyan: `#00ffff`
- Green: `#00ff00`
- Magenta: `#ff00ff`
- Red: `#ff0000`
- Blue: `#0000ff`

## Technical Details

- **Aspect Ratio**: 16:9 (standard HD)
- **Z-Index Hierarchy**: 
  - Center black bar: 200 (highest)
  - Timers: 10
  - Squares: 10
  - Corner circles: 4
  - Central circle: 3
  - Background: 1-2
- **Responsive Breakpoint**: 768px (mobile adjustments)

## Features in Detail

### Timer Display
- Two digital timers split by the center black bar
- Left timer: Time format (HH:MM) with blinking colon
- Right timer: Date format (DD-MM-YY)
- Updated via JavaScript

### Square Grids
- Main grid: 20 squares (10 left, 10 right) below timers
- Center squares: 4 squares inside the center black bar
- White borders for contrast testing

### Grayscale Gradient
- 10 shades progressing from black to white
- Used for brightness and contrast calibration
- Evenly distributed across the gradient

## Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

## License

This project is open source and available for educational and personal use.

## Credits

Created as a recreation of classic television test patterns used for display calibration and signal testing.

---

**Note**: This is a static web implementation. For actual display calibration, use professional calibration tools and test patterns.

