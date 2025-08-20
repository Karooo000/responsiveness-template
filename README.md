# Responsive Design Template

A comprehensive CSS media query template organized by aspect ratio and screen width breakpoints for responsive web design. **This template is designed as a website builder addon** to help developers create responsive layouts efficiently. **This template covers 100% of screen sizes, from extreme ultra-wide displays (5120px+) down to the smallest devices like Apple Watch (300px and below).**

## Overview

This template provides a systematic approach to responsive design using CSS media queries. It's organized by aspect ratio first, then by screen width, making it easy to target specific device orientations and sizes. **The template includes gaps where you can add width-based media queries for your website builder.** This is a **desktop-first approach** where styles cascade down from larger screens to smaller ones.

## Structure

The template is organized into three main aspect ratio categories:

### Wide screens (min-aspect-ratio: 1920/878) - Aspect Ratio: 2.19+

- No width constraint (general wide screens)
- XXL (1920px+) - Ultra-wide monitors, 4K displays
- XL (up to 1920px) - Standard desktop monitors
- L (up to 1280px) - Small desktop, large laptops
- M (up to 991px) - Tablets in landscape, small laptops

**Use your website builder to add styles between here**

### Square to tall (max-aspect-ratio: 1920/1240) - Aspect Ratio: 1.55 to 2.19

- **General square media query (no width constraint)** - Standard tablets, square monitors
- XXL (1920px+) - Large square displays
- XL (up to 1920px) - Standard square monitors
- L (up to 1280px) - Small square displays
- M (up to 991px) - Tablets in portrait, small square screens
- XS (up to 479px) - Large phones in landscape
- XXS (up to 420px) - Standard phones in landscape

### Tall (max-aspect-ratio: 1920/2050) - Aspect Ratio: 0.94 and below

- No width constraint (general tall screens) - Mobile phones, portrait tablets
- XXL (1920px+) - Ultra-tall displays
- XL (up to 1920px) - Tall desktop monitors
- L (up to 1280px) - Tall laptop screens
- M (up to 991px) - Tablets in portrait
- S (up to 767px) - Large phones
- S (up to 479px) - Standard phones
- XXS (up to 420px) - Small phones
- XXXS (up to 300px) - Very small devices

## Breakpoint Sizes with Device Examples

- **XXL**: 1920px and above - Ultra-wide monitors, 4K displays, large desktop screens
- **XL**: Up to 1920px - Standard desktop monitors, large laptops
- **L**: Up to 1280px - Small desktop monitors, large laptops, some tablets
- **M**: Up to 991px - Tablets in landscape, small laptops, large phones in landscape
- **S**: Up to 767px - Tablets in portrait, large phones
- **XS**: Up to 479px - Standard phones, small tablets
- **XXS**: Up to 420px - Small phones, compact devices
- **XXXS**: Up to 300px - Very small devices, smartwatches

## Website Builder Integration

**This template is specifically designed as a website builder addon.** The structure allows you to:

1. **Add width-based media queries** in the designated gaps for your website builder
2. **Use aspect ratio queries** for orientation-specific layouts
3. **Combine both approaches** for comprehensive responsive design
4. **Maintain consistency** across different screen sizes and orientations

## Usage

1. **Copy the template** into your CSS file or HTML `<style>` tag
2. **Add width-based styles** in the designated gaps for your website builder
3. **Add responsive styles** inside each media query block
4. **Organize by component** - group related styles together within each breakpoint
5. **Test across devices** to ensure proper responsive behavior

## Example

```css
/* Wide screens - landscape orientation */
@media (min-aspect-ratio: 1920/878){
    .hero-section {
        height: 100vh;
        display: flex;
    }
    
    .content {
        width: 60%;
        margin: 0 auto;
    }
}

/* General square orientation - no width constraint */
@media (max-aspect-ratio: 1920/1240) {
    .hero-section {
        height: auto;
        min-height: 80vh;
    }
}

/* Mobile devices - portrait orientation */
@media (max-width: 767px) and (max-aspect-ratio: 1920/2050){
    .hero-section {
        height: auto;
        min-height: 100vh;
        flex-direction: column;
    }
    
    .content {
        width: 100%;
        padding: 20px;
    }
}
```

## Benefits

- **Organized by orientation**: Easier to manage landscape vs portrait layouts
- **Website builder friendly**: Designed specifically for website builder integration
- **Desktop-first approach**: Styles cascade down from larger to smaller screens
- **Maintainable**: Clear structure makes it easy to find and modify styles
- **Comprehensive coverage**: Covers all common device sizes and orientations
- **Flexible**: Can be easily customized for specific project needs

## Browser Support

This template uses standard CSS media queries that are supported by all modern browsers:
- Chrome 21+
- Firefox 3.5+
- Safari 4+
- Edge 12+
- Internet Explorer 9+

## License

This template is provided as-is for educational and development purposes. Feel free to modify and use in your projects.
