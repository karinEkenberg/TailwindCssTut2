# Tailwind CSS Tutorial

This project is a simple setup for learning and practicing Tailwind CSS. It follows a tutorial to demonstrate how to configure Tailwind in a project and apply it to styling web pages.

## Project Overview

The project uses **Tailwind CSS** for utility-first styling. The configuration includes tools to automate CSS generation and formatting with Prettier.

### Main Files

- **`tailwind.config.js`**: Configures the content path for Tailwind to scan and defines the theme settings.
- **`package.json`**: Includes scripts for running Tailwind and Prettier, and specifies the dependencies used.
- **`package-lock.json`**: Auto-generated file to ensure consistent installation of the exact versions of dependencies.

### Scripts

- `npm run tailwind`: Watches for changes in the `src/input.css` file and compiles the CSS into `build/css/style.css`.
- `npm run prettier`: Formats all `.html` files in the project using Prettier, with Tailwind-specific plugin configuration.

## Installation and Setup

1. Clone the repository.
2. Run `npm install` to install the necessary dependencies.
3. To start the Tailwind CSS watcher, run:

   ```bash
   npm run tailwind
   ```

   This will generate the CSS file and watch for changes.

4. If you need to format the HTML files, run:

   ```bash
   npm run prettier
   ```

## Tailwind Configuration

The **`tailwind.config.js`** file is configured to scan all HTML files in the `build` folder for class names. You can modify this if you add more paths or content types.

```javascript
module.exports = {
  content: ["./build/*.html"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

## Dependencies

- **Tailwind CSS**: Utility-first CSS framework.
- **Prettier Plugin for Tailwind CSS**: Ensures that Tailwind classes are properly formatted.
