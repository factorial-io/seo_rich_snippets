A custom Drupal Module which provides rich snippets for search engine.

## Installation

Follow procedure to install a drupal module.
You may use this [link for docmentation on Drupal.org](https://www.drupal.org/docs/7/extend/installing-modules) to know more about how to install modules.

## Configuration

Visit admin/config/system/site-rich-snippets to configure.

## Usage

### PHP Templates.
Rich snippets are available in `$variables['page']['content']['seo_rich_snippets']` in `page.tpl.php`.


In case `$variables['page']['content']` is not printed on page, you might have to print the snippets explicitely by doing so,

`<?php drupal_render($variables['page']['content']['seo_rich_snippets']); ?>`

### Twig Templates
In case of Twig templates use the following equivalent syntax in the page template,

`{{ page.content.seo_rich_snippets|raw }}`

### BreadcrumbList

BreadcrumbList are automatically picked up drupal_get_breadcrumbs.
