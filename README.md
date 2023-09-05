# The Primer theme

## Usage

To use the Primer theme:

1. Add the following to your site's `_config.yml`:

   ```yml
   remote_theme: pages-themes/primer@v0.2.0
   plugins:
     - jekyll-remote-theme # add this line to the plugins list if you already have one
   ```

## Customizing

### Configuration variables

Primer will respect the following variables, if set in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
google_analytics: [Your Google Analytics tracking ID]
```

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site
2. Add the following content to the top of the file, exactly as shown:

   ```scss
   ---
   ---

   @import '{{ site.theme }}';
   ```

3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

### Previewing the theme locally

If you'd like to preview the theme locally (for example, in the process of proposing a change):

1. Clone down the theme's repository (`git clone https://github.com/pages-themes/primer`)
2. `cd` into the theme's directory
3. Run `script/bootstrap` to install the necessary dependencies
4. Run `bundle exec jekyll serve` to start the preview server
5. Visit [`localhost:4000`](http://localhost:4000) in your browser to preview the theme
