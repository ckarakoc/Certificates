# AGENTS.md

This repository is a certificate showcase using Jekyll for GitHub Pages deployment. It contains primarily static content (certificate images and documentation) rather than a traditional codebase.

## Repository Structure

- `README.md` - Main documentation with certificate tables
- `pdf/` - Directory containing PDF certificates
- `*.jpg`, `*.png`, `*.svg` - Certificate images in root directory
- `.github/workflows/jekyll-gh-pages.yml` - GitHub Actions workflow for Jekyll deployment

## Build and Deployment Commands

### Jekyll Development
```bash
# Install Jekyll and dependencies (if needed)
gem install jekyll bundler

# Serve locally for development
bundle exec jekyll serve

# Build the site
bundle exec jekyll build
```

### GitHub Actions Deployment
The site is automatically deployed to GitHub Pages when pushing to the `master` branch via the workflow in `.github/workflows/jekyll-gh-pages.yml`.

## Content Guidelines

### File Naming
- Use descriptive names for certificate images
- Include platform/provider prefix (e.g., `UC-` for Udemy, `AZ-` for Azure)
- Use consistent UUID-based naming for Udemy certificates
- Keep filenames under 255 characters

### Image Formats
- Use `.jpg` for photograph-style certificates
- Use `.png` for certificates with text/sharp edges
- Use `.svg` for vector-based certification badges
- Store PDF versions in the `pdf/` directory

### README.md Structure
- Follow the existing table format for certificates
- Include repository links for related projects
- Use consistent image width (100px recommended)
- Maintain proper markdown table alignment

## Jekyll Configuration

This repository uses Jekyll for GitHub Pages. Key considerations:
- No custom Jekyll configuration files present
- Uses default Jekyll settings
- Source directory: `./`
- Destination: `./_site` (build output)

## Git Workflow

- Main branch: `master`
- Push to master triggers automatic deployment
- No build scripts or package managers in use
- Standard git workflow applies

## File Organization

### Root Level
- Certificate images (JPG, PNG, SVG)
- README.md (main documentation)
- .gitignore (standard ignore patterns)

### PDF Directory
- All PDF certificates stored in `pdf/` directory
- Mirror the naming convention of root-level images

### GitHub Configuration
- Workflow file in `.github/workflows/`
- Standard GitHub Pages permissions configured

## Development Notes

- This is a static content repository, not a traditional codebase
- No testing framework required
- No linting or formatting tools needed
- Focus on content organization and presentation
- Maintain consistent table formatting in README.md

## Common Tasks

### Adding New Certificates
1. Add image file to root directory
2. Add PDF version to `pdf/` directory (if available)
3. Update README.md table with new entry
4. Follow existing format and naming conventions

### Updating Documentation
- Edit README.md directly
- Test table formatting
- Ensure all image links are valid
- Maintain consistent styling

### Deployment
- Push changes to master branch
- GitHub Actions will automatically build and deploy
- No manual deployment steps required