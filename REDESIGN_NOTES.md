# Black & gold redesign

This version retains the original AcademicPages/Jekyll site and its content collections, while introducing a dark editorial design inspired by Temple's restrained, immersive visual language.

## Changed files
- `_pages/about.md`: rebuilt homepage with hero, about, research, featured publication, academic journey and contact sections.
- `_sass/_luxury.scss`: new responsive black/champagne-gold design system, including inner pages.
- `assets/css/main.scss`: imports the new stylesheet last, to override the original theme.
- `_includes/masthead.html`: custom wordmark/navigation.
- `_includes/footer.html`: minimal footer.
- `_includes/head/custom.html`: font loading and dark browser theme.
- `_data/navigation.yml`: updated site navigation.

## Deploy
Push the repository contents to your GitHub Pages repository's publishing branch. GitHub Pages should build the site as before. Keep `_sass/_luxury.scss` and the added import in `assets/css/main.scss` together.

## Optional refinements
- Replace the existing portrait at `images/Auddya_Debabrata_03.jpg` if desired.
- Edit homepage text and research cards in `_pages/about.md`.
- Change gold shade using `--lux-gold` in `_sass/_luxury.scss`.
- Font files are not bundled; Google Fonts are loaded via the head include and serif/system fallbacks are provided.

## Verification
File structure and homepage section tags were checked. A Jekyll build was not executed because Ruby/Bundler were unavailable in this environment. Preview with `bundle exec jekyll serve` locally before pushing.
