# React Boilerplate with Vite

## Table of Contents

1. [Introduction](#introduction)
2. [Folder Structure](#folder-structure)
3. [Getting Started](#getting-started)
4. [Usage Guidelines](#usage-guidelines)

---

## Introduction

Welcome to the README for our Vite-React boilerplate. We use an opinionated structure that aims for maintainability, ease of navigation, and adheres to best practices in both React and SCSS. It serves as a quick starting point for new projects.

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
                    Vendors/            # 3rd-party vendor scripts
                        [Vendor Files]
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
