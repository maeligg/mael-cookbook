# Maël's cookook

This is my own online cookbook, based on [My Online Cookbook](https://github.com/maeligg/my-online-cookbook). It's available at https://mael-recettes.netlify.app/

## Running the site locally

1. `npm install` to install all dependencies
2. `npm run dev` to serve the site locally
3. `npm run build` to build the site for production

## Access the CMS admin interface

Go to `/admin` to access the admin interface (this also works locally). You'll need to configure a user with [Netlify Identity](https://docs.netlify.com/visitor-access/identity/) to log in. For more information on how to use or configure Netlify CMS go to [their documentation](https://www.netlifycms.org/docs/intro/). In addition to recipes, all site settings (primary color, etc) as well as labels are editable from this interface.

## Directory structure

- `.eleventy.js` has all the custom configuration for [Eleventy](https://11ty.io), including collections, filters and shortcodes.
- `src/_data` contains nav and site settings, also editable from the CMS admin interface.
- `src/_includes` contains layouts and reusable components (including SVG icons).
- `src/admin` contains the configuration for editable fields in Netlify CMS.
- `src/img` contains all images. Note that only images placed in `src/img/recipes` are editable from the CMS admin interface.
- `src/recipes` is your main content, with each recipe saved as a markdown file.
- Each other page is located at the root of `src/` as its own markdown or nunjucks file.
