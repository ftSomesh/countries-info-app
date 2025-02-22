# Country Info App

A web application that displays country details with a 
skeleton loading effect before content is fully loaded.

## Features

- Fetches and displays country details (flag, name, population, etc.)
- Implements a skeleton loading effect for smooth UI experience
- Supports both light and dark mode for skeleton loaders
- Optimized skeleton effect for images and text separately

## Technologies Used

- HTML
- CSS (with custom properties for light/dark mode support)
- JavaScript (DOM manipulation, event handling, and dynamic class updates)

## Project Structure

```
root/
├── images       # Favicon Image
├── index.html       # Main HTML structure
├── style.css        # Styling and skeleton loader effect
├── script.js        # JavaScript functionality
├── country.html       # Secondary HTML structure
├── country.css        # Secondary Css File
├── country.js        # Secondary Script File
└── README.md        # Project documentation

```

## How It Works

1. **Skeleton Loader**: Placeholder elements are shown before the actual content loads.
2. **Fetching Data**: Country details are loaded dynamically.
3. **Removing Skeleton Effect**:
   - Text: `classList.remove("skeleton")` is used once content is ready.
   - Skeleton Effect: A wrapper (`.skeleton`) is used with a `::before` effect, removed after loading.
4. **Dark Mode Support**: Custom CSS variables ensure proper skeleton colors in both modes.

## Installation & Setup

1. Clone the repository:
   ```sh
   git clone https://github.com/ftSomesh/country-info-app.git
   ```
2. Navigate to the project folder:
   ```sh
   <!-- Undefined -->
   ```
3. Open `index.html` in a browser.

## Customization

- Modify `--var-skeleton-color-first`, `--var-skeleton-color-second`, `--var-skeleton-color-third` in `style.css` to customize the skeleton loader colors.
- Adjust the image skeleton effect by modifying `.image-wrapper::before` in `style.css`.

## Known Issues & Fixes

### **Skeleton Effect Not Disappearing**

- Ensure `classList.remove("skeleton")` is applied after content is loaded.
- JavaScript should listen to the `load` event of images before removing the effect.

## Future Enhancements

- Add API integration for dynamic country data
- Implement a toggle switch for dark/light mode
- Improve performance with lazy loading

## License

This project is open-source and free to use.

## Author
- **Full Name** : Somesh Kumar Sahu
- **Email** : desktopsomesh@gmail.com  
- **Github** : https://github.com/ftSomesh  

---

Made with ❤️ by `Someshhh`
