# Multi Font CSS

A simple, efficient solution for integrating multiple custom web fonts into your project using CSS and SCSS. This repository includes multiple font families that can be used by simply linking a single CSS file to your project.

## Table of Contents

1. [Features](#features)
2. [Installation](#installation)
3. [How It Works](#how-it-works)
4. [Future Improvements](#future-improvements)
5. [Contributing](#contributing)
6. [License](#license)
7. [Acknowledgments](#acknowledgments)

## Features

- Supports multiple font families with separate font-face declarations for each.
- Uses SCSS for easier management and bundling of CSS files.
- Simple setup and integration into any web project.
- No external dependencies required, all font files are self-contained.
- Fast and efficient integration of fonts without the need for additional HTTP requests.

## Installation

1. **Clone the repository** to your local machine:

```bash
git clone https://muhammad-aqib-bashir.github.io/multi-font-css.git
cd multi-font-css
```

2. **Install the required dependencies** using npm:

```bash
npm install
```

This will install all necessary packages, including SCSS and dependencies required for compiling.

## How It Works

1. The `index.scss` file imports all font-face declarations from individual font files (e.g., `abc-ginto.css`).
2. Once the SCSS is compiled using `npm run build-css`, the final `index.css` file is generated.
3. The `index.css` file is ready to be included in any HTML page, making all the fonts available for use.

To use the fonts in your web project, link the `index.css` file in your HTML `<head>` section:

```html
<link
  rel="stylesheet"
  href="https://muhammad-aqib-bashir.github.io/multi-font-css/index.css"
/>
```

Additionally, if you're using SCSS in your project, simply import the font family (e.g., `abc-ginto.css`) file into your own SCSS file:

```scss
@use "https://muhammad-aqib-bashir.github.io/multi-font-css/css/abc-ginto.css";
```

### Building the CSS

To compile SCSS files and generate the final CSS:

```bash
npm run build-css
```

This command will compile the SCSS files and generate the `index.css` file in the root directory, which can be linked to your project.

## Future Improvements

- **Add More Font Families**: The repository will be expanded with more font families in the future.
- **Customization**: Provide options for customizing fonts or creating dynamic imports for multiple configurations.
- **Optimized Font Loading**: Integrate `font-display` property for better font loading performance.

## Contributing

Contributions are welcome! Feel free to fork the repository, make changes, and submit pull requests. To contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the developers of SCSS and the web font community for providing resources and libraries.
- Special thanks to contributors and open-source projects that have helped in making this project better.
