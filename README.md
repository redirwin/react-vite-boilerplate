# React Boilerplate with Vite

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Folder Structure](#folder-structure)
4. [Usage Guidelines](#usage-guidelines)
5. [npm Packages](#3rd-party-npm-packages)
6. [Scripts Directory](#scripts-directory)

---

## Introduction

Welcome to the README for our Vite-React boilerplate. We use an opinionated structure that aims for maintainability, ease of navigation, and adheres to best practices in both React and SCSS. It serves as a quick starting point for new projects.

---

## Getting Started

### Pre-requisites

- Vite, Node.js, and npm installed on your system.

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/your-username/vite-react-boilerplate.git my-new-app
   ```

   Navigate to the project's directory:

   ```bash
   cd my-new-app
   ```

2. **Install Dependencies**:

   ```bash
   npm install
   ```

3. **Personalize**: Update the `package.json` and README to your project's specifics.

4. **Run the Project**:

   ```bash
   npm run dev
   ```

You're all set for development! The server reloads automatically upon file changes.

---

## Folder Structure

Here's an overview of the folder structure used:

```
Project Root
    index.html                      # Main HTML file (entry point)
        src/                            # Source code directory
            assets/                     # Static assets like images, fonts, etc.
                logo.png                # Example logo image
            components/                 # React components
                layout/                 # Layout components
                    Footer/
                        Footer.jsx
                        Footer.module.scss
                    [More Layout Components]
                modules/                # Modular, reusable components
                    PriceTable/
                        PriceTable.jsx
                        PriceTable.module.scss
                    [More Modular Components]
                templates/              # Template components
                    BlogList/
                        BlogList.jsx
                        BlogList.module.scss
                    [More Template Components]
            global/                     # Global resources
                scripts/                # Global JS scripts
                styles/                 # SCSS styles
                    1 - Helpers/          # Helper styles (variables, functions, mixins)
                        [Helper Files]
                    2 - Plugins/          # 3rd-party plugin styles
                        [Plugin Files]
                    3 - Base/           # Base styles (global, typography, etc.)
                        [Base Files]
            App.jsx                     # Root React component
            main.jsx                    # Initializes and renders React app
            main.scss                   # Main SCSS file (imports all global SCSS files)
```

## Usage Guidelines

### Adding a New Component

1. Go to the `src/components/` directory.
2. Choose the appropriate subfolder (`layout`, `modules`, or `templates`).
3. Create a new folder using PascalCase.
4. Create a `.jsx` and `.module.scss` file inside, named after the folder.
5. Use PascalCase for all names. For example, `MyComponent.jsx` and `MyComponent.module.scss`.
6. When building scss modules, the main class name should also use PascalCase. For example, `.MyComponent { ... }`.

**Feel free to change, remove, or add to any out-of-the-box components within the primary folders, but DO NOT change the primary folder names (layout, modules, templates).**

### Adding Global Styles

1. Navigate to `src/global/styles/`.
2. Choose the appropriate subfolder and update the `.scss` files as needed.

**For global styles, use the existing files and DO NOT change the file names, but change the styles as the project dictates.**

## 3rd-party npm Packages

We've vetted certain npm packages for quality, ease of use, and long-term support. You are encouraged to use these packages when they fit your needs. For more information about npm and how to manage npm packages, you can read the [npm documentation](https://docs.npmjs.com/about-npm).

The list of approved packages will be continuously updated:

- [`axios`](https://www.npmjs.com/package/axios) for HTTP requests.
- [`formik`](https://www.npmjs.com/package/formik) for form handling.
- [`yup`](https://www.npmjs.com/package/yup) for form validation.
- [`react-query`](https://www.npmjs.com/package/@tanstack/react-query) for data fetching, caching, and state management.
- [`react-router-dom`](https://www.npmjs.com/package/react-router-dom) for routing.

## Scripts Directory

The `scripts` folder inside the `src/global/` directory is intended for extra JavaScript that doesn't fit into the React component structure or doesn't come as an npm package. For example, if you need to add a custom script to the `index.html` file, you can add it to `scripts/index.js` and import it in `index.html`.

**This should be used sparingly.**
