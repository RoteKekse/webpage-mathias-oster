# Mathias Oster - Academic Website

This is the source repository for the academic website of Prof. Dr. Mathias Oster, Junior Professor of Mathematics at RWTH Aachen University.

## Website Structure

The website is built using [MkDocs](https://www.mkdocs.org/) with the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme.

### Sections

- **About**: Introduction and research interests
- **Publications**: List of academic publications with Google Scholar integration
- **CV & Education**: Academic background, positions, and qualifications
- **Research Cooperations**: Collaborative projects and partners
- **Contact**: Office hours, contact information, and location
- **Impressum**: Legal notice and privacy policy

## Local Development

### Prerequisites

- Python 3.x
- pip

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/website_mathias.git
   cd website_mathias
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running Locally

Start the development server:

```bash
mkdocs serve
```

The site will be available at `http://127.0.0.1:8000/`

The development server supports live reloading, so changes to the content will be reflected immediately.

### Building

To build the static site:

```bash
mkdocs build
```

The built site will be in the `site/` directory.

## Deployment

The website is automatically deployed to GitHub Pages using GitHub Actions whenever changes are pushed to the `main` branch.

### Setup GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" in the left sidebar
3. Under "Build and deployment", select:
   - **Source**: GitHub Actions
4. Push to the `main` branch to trigger deployment

The site will be available at: `https://yourusername.github.io/website_mathias/`

### Manual Deployment

You can also manually trigger the deployment:

1. Go to the "Actions" tab in your GitHub repository
2. Select the "Deploy MkDocs to GitHub Pages" workflow
3. Click "Run workflow"

## Customization

### Colors

The site uses an eggshell/rose color scheme defined in:
- [`docs/stylesheets/extra.css`](docs/stylesheets/extra.css)

### Configuration

Main configuration file:
- [`mkdocs.yml`](mkdocs.yml)

### Content

All content pages are in Markdown format in the `docs/` directory:
- `docs/index.md` - About page
- `docs/publications.md` - Publications
- `docs/cv.md` - CV and Education
- `docs/cooperations.md` - Research Cooperations
- `docs/contact.md` - Contact Information
- `docs/impressum.md` - Legal Notice

## Google Scholar Integration

The publications page includes a link to Google Scholar. To integrate your profile:

1. Create a Google Scholar profile at https://scholar.google.com/citations
2. Get your user ID from your profile URL
3. Update the links in:
   - `docs/publications.md`
   - `docs/contact.md`
   - `mkdocs.yml` (in the `extra.social` section)

Note: Google Scholar does not provide a direct API for automatically fetching publications. The current implementation links to your profile where publications are automatically updated by Google.

## Adding Publications

While Google Scholar maintains an up-to-date list automatically, you can manually curate publications on the website:

1. Edit [`docs/publications.md`](docs/publications.md)
2. Add entries following the existing format
3. Include links to PDFs, DOIs, and arXiv preprints as available

## Technologies Used

- **MkDocs**: Static site generator
- **Material for MkDocs**: Modern theme with excellent features
- **GitHub Actions**: Automated deployment
- **GitHub Pages**: Free hosting for the website

## License

The content of this website is © Mathias Oster. The MkDocs configuration and structure can be reused under the MIT License.

## Contact

For questions or issues with this website, please contact:
- Email: mathias.oster@rwth-aachen.de
- GitHub Issues: [Report an issue](https://github.com/yourusername/website_mathias/issues)

---

*Last updated: January 2026*
# webpage-mathias-oster
