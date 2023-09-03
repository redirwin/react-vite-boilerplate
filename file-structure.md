```
Project Root
    ├── index.html                      # Main HTML file (entry point)
    └── src/                            # Source code directory
        ├── assets/                     # Static assets like images, fonts, etc.
        │   └── logo.png                # Example logo image
        ├── components/                 # React components
        │   ├── layout/                 # Layout components
        │   │   └── Footer/
        │   │       ├── Footer.jsx
        │   │       └── Footer.module.scss
        │   │   └── [More Layout Components]
        │   ├── modules/                # Modular, reusable components
        │   │   └── PriceTable/
        │   │       ├── PriceTable.jsx
        │   │       └── PriceTable.module.scss
        │   │   └── [More Modular Components]
        │   └── templates/              # Template components
        │       └── BlogList/
        │           ├── BlogList.jsx
        │           └── BlogList.module.scss
        │       └── [More Template Components]
        ├── global/                     # Global resources
        │   ├── scripts/                # Global JS scripts
        │   └── styles/                 # SCSS styles
        │       ├── 1 - Helpers/          # Helper styles (variables, functions, mixins)
        │       │   └── [Helper Files]
        │       ├── 2 - Plugins/          # 3rd-party plugin styles
        │       │   └── [Plugin Files]
        │       └── 3 - Base/           # Base styles (global, typography, etc.)
        │           └── [Base Files]
        ├── App.jsx                     # Root React component
        ├── main.jsx                    # Initializes and renders React app
        └── main.scss                   # Main SCSS file (imports all global SCSS files)
```
