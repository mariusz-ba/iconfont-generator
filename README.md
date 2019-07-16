# Iconfont generator
This app generates iconfont from provided svg icons. In addition it creates `icons.scss` file that contains map with all icons unicodes.

## Installation and usage
Install needed dependencies
```bash
npm install
```
Copy your svg icons to `src/assets/icons` directory and run:
```bash
npm run build
```
This will generate two output directories
1. `dist/fonts/iconfont` - Includes all fonts in different formats.

    Genereated font files:
    ```
    iconfont.ttf
    iconfont.eot
    iconfont.woff
    iconfont.woff2
    ```
2. `dist/icons/icons.scss` - Scss file with map containing all icons unicodes.

    Example `icons.scss` output:
    ```scss
    $icons: (
      icon-avatar: "\EA01",
      icon-envelope: "\EA02",
      icon-phone-call: "\EA03"
    )
    ```
    Later they can be used in `scss` styles like so:
    ```scss
    .icon::before {
      font-family: 'iconfont';
      content: map-get($icons, 'icon-avatar');
    }
    ```
