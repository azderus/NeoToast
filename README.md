# NeoToast

A lightweight, modern toast notification system with smooth animations and progress bars. Created by Azderus.

## Description

NeoToast is a next-generation toast notification library that combines modern aesthetics with powerful functionality. Built with a focus on user experience, it features a sleek dark-themed design with glass morphism effects, smooth animations, and an intuitive progress system. Perfect for developers who want to add elegant, non-intrusive notifications to their web applications without the bloat of larger libraries.

Key highlights:
- Zero dependencies
- Only 5KB minified
- Built-in TypeScript support
- Modern glass morphism design
- Smart toast stacking
- Progress indication with pause/resume
- Promise-based operations support

![Toast Preview](preview.gif)

## Features

- 🎨 Modern, clean design with blur effects
- 🚀 Smooth animations and transitions
- ⏱️ Progress bar with pause on hover
- 🎯 Multiple toast types (success, error, info)
- 📱 Fully responsive design
- 🔄 Promise support
- 🎭 Stack management (max 3 visible toasts)
- ⚡ Lightweight and dependency-free

## Installation

1. Download `NeoToast.js` file
2. Add it to your project
3. Include the script in your HTML:

```html
<script src="path/to/NeoToast.js"></script>
```

Alternatively, use the CDN:

```html
<script src="https://cdn.jsdelivr.net/gh/azderus/NeoToast@main/NeoToast.js"></script>
```

## Usage

### Basic Usage

```javascript
// Success notification
toast.success('Operation completed successfully!');

// Error notification
toast.error('Something went wrong!');

// Info notification
toast.info('Here is some information');
```

### Custom Duration

```javascript
// Custom duration in milliseconds (default is 4000ms)
toast.success('Custom duration toast', 5000);
```

### Promise Support

```javascript
// Show loading state while promise is pending
toast.promise(asyncOperation(), {
    loading: 'Loading...',
    success: 'Operation completed!',
    error: 'Operation failed!'
});
```

### Manual Control

```javascript
// Create a toast that doesn't auto-dismiss
const toastElement = toast.show('Manual close toast', 'info', 0);

// Remove it later
toast.remove(toastElement);
```

## Customization

You can customize the appearance by modifying the CSS variables:

```css
:root {
    --toast-success: #10b981;  /* Success color */
    --toast-error: #ef4444;    /* Error color */
    --toast-info: #3b82f6;     /* Info color */
    --toast-bg: rgba(0, 0, 0, 0.7);  /* Toast background */
    --text-color: #ffffff;     /* Text color */
    --toast-border: rgba(255, 255, 255, 0.1);  /* Border color */
}
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

Note: Backdrop filter effect might not work in all browsers.

## License

MIT License - feel free to use in your projects

## Author

Created by Azderus
- GitHub: [@azderus](https://github.com/azderus)

## Contributing

Feel free to submit issues and enhancement requests!
