# Iconfont generator
This app generates iconfont from provided svg icons. In addition it creates `icons.scss` file that contains map with all icons unicodes.

# Installation and usage
Install needed dependencies
```bash
npm install
```
Copy your svg icons to `src/assets/icons` directory and run:
```bash
npm run build
```
This will generate two output directories
- `dist/fonts/iconfont` - Includes all fonts in different formats
- `dist/icons/icons.scss` - Scss file with map containing all icons unicodes that can later be used in `content: "unicode"`