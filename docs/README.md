# Halloween - GitHub Pages Site

This directory contains a Jekyll-based GitHub Pages site for the book.

## Local Development

1. Install Ruby and Bundler if not already installed
2. Install dependencies:
   ```bash
   bundle install
   ```

3. Run local server:
   ```bash
   bundle exec jekyll serve
   ```

4. Visit: http://localhost:4000

## Deploy to GitHub Pages

1. Create a new repository on GitHub
2. Push this directory to the repository
3. Go to Settings > Pages
4. Set source to main branch / root folder
5. Your site will be published at: https://username.github.io/repository/

## Customization

- Edit `_config.yml` to change site settings
- Modify `_layouts/default.html` to customize the layout
- Change the theme in `_config.yml` and `Gemfile`

## Available Themes

- jekyll-theme-cayman (default)
- minima
- jekyll-theme-minimal
- just-the-docs (great for documentation)

To change theme, update both `_config.yml` and `Gemfile`, then run `bundle install`.
