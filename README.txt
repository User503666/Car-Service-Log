AutoLog - updated category navigation

Files included:
- index.html: complete updated app based on the newer uploaded index(3).html
- manifest.json: manifest supplied by the user
- sw.js: updated service worker with safer local asset caching

Navigation behavior:
1. The first screen shows main service categories only.
2. Selecting a category shows only that category's subcategories.
3. Selecting a subcategory shows the individual service checkboxes.
4. Back buttons move between the three levels.
5. Search continues to search all categories, subcategories, and services.

Before publishing to GitHub Pages, also add the icon files referenced by manifest.json:
- icon-192.png
- icon-512.png

The original app loads Tailwind CSS from its CDN, so the first load and styling refresh require internet access. Offline availability of app logic is improved by sw.js, but Tailwind itself is not bundled locally in this package.

Validation performed:
- JavaScript syntax check for the main index.html script
- JavaScript syntax check for sw.js
- JSON parse check for manifest.json

This package is based on the currently available index(3).html source. It does not yet include any of the remaining project files or icon images that have not been uploaded in this conversation.
