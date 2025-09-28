# 🛡️ DevSecOps Bootcamp Documentation ♾️

A modern, responsive documentation site built with MkDocs and the Material theme.

## Features

- **Modern Design**: Clean, responsive layout with Material Design principles
- **Dark/Light Mode**: Toggle between dark and light themes
- **Search Functionality**: Full-text search with highlighting and suggestions
- **Code Highlighting**: Syntax highlighting with copy-to-clipboard functionality
- **Navigation**: Tabbed navigation with sections and smooth scrolling
- **Mobile Responsive**: Optimized for all device sizes

## Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

## Installation

1. Clone this repository:
   ```bash
   git clone <your-repo-url>
   cd mkdocs-project
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Local Development

To start the development server:
```bash
mkdocs serve
```

The site will be available at `http://localhost:8000`

### Building the Site

To build the static site:
```bash
mkdocs build
```

The built site will be in the `site/` directory.

### Deploying

To deploy to GitHub Pages:
```bash
mkdocs gh-deploy
```

## Project Structure

```
mkdocs-project/
├── docs/
│   ├── index.md          # Home page
│   ├── getting-started.md
│   ├── user-guide.md
│   ├── api-reference.md
│   └── about.md
├── site/                 # Built site (generated)
├── mkdocs.yml           # MkDocs configuration
├── requirements.txt     # Python dependencies
└── README.md           # This file
```

## Configuration

The site is configured through `mkdocs.yml` which includes:

- **Theme**: Material theme with custom color schemes
- **Navigation**: Organized into logical sections
- **Extensions**: Enhanced markdown support with:
  - Admonitions
  - Code highlighting
  - Tabbed content
  - Table of contents with permalinks
- **Plugins**: Search and HTML minification

## Customization

### Adding New Pages

1. Create a new `.md` file in the `docs/` directory
2. Add the page to the `nav:` section in `mkdocs.yml`

### Changing Theme Colors

Edit the `palette:` section in `mkdocs.yml` to customize colors.

### Adding New Features

The Material theme supports many extensions. See the [Material for MkDocs documentation](https://squidfunk.github.io/mkdocs-material/) for more options.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally with `mkdocs serve`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For questions or issues, please open an issue on the GitHub repository.
