# Show Only Posts in Search (Exclude Tags)

A WordPress plugin to show only posts in search results, excluding pages, posts with specific tags, and posts from specific categories.

## Features

- Only displays published posts in WordPress search results.
- Excludes pages, custom post types, and drafts/private posts from search.
- Excludes posts with specific tag IDs (`1394`, `1396`, `1703`, `1398`).
- Excludes posts from the `homeschool` and `lifestyle` categories.
- Completely blocks category and tag archive pages from appearing in search results.
- Removes categories and tags from search suggestions/autocomplete.

## Installation

1. Download or clone this repository.
2. Upload `disablesearch.php` to your WordPress site's `wp-content/plugins/` directory.
3. Activate the plugin from the WordPress admin dashboard.

## How It Works

- Hooks into the WordPress search query to:
  - Restrict results to published posts only.
  - Exclude posts with certain tags and from certain categories.
- Prevents category and tag archive pages from being shown in search results (returns a 404 for those).
- Removes taxonomy terms from search suggestions and autocomplete.

## Customization

- To change excluded tag IDs, edit the `$excluded_tag_ids` array in [`disablesearch.php`](c:/Users/AQIB%20AHMED/AppData/Local/Temp/e86252ea-70e2-44f5-a247-1302c302fb97_Disable%20Search%20Showit.zip.b97/disablesearch.php).
- To change excluded categories, update the slugs in the `get_category_by_slug` calls.

## License

GPL2

---

**Author:** sajid