Crec que l'he de posar a /var/www/hola.com/themes/custom

Si vols crear un tema ràpid et pots ajudar de:
php core/scripts/drupal generate-theme my_new_theme

La típica estructura seria:

-
|-my_new_theme.breakpoints.yml // Temes de responsiveness...
|-my_new_theme.info.yml // El més important, on defineixes...
|-my_new_theme.libraries.yml // The .libraries.yml file is used to DEFINE! JavaScript and CSS libraries that can be loaded by the theme.
|-my_new_theme.theme // The .theme file is a PHP file that contains all the conditional logic and data (pre)processing of the output.
|-config
|  |-install
|  |  |-my_new_theme.settings.yml
|  |-schema
|  |  |-my_new_theme.schema.yml
|-css
|  |-my_new_theme.css
|-js
|  |-my_new_theme.js
|-images
|  |-buttons.png
|-logo.svg
|-screenshot.png
|-templates
|  |-maintenance-page.html.twig
|  |-node.html.twig // You can override core templates by following specific naming conventions based on what you're overriding. For example:
    To override the default node template for the article content type, use node--article.html.twig.
    To override a specific block, use block--BLOCKNAME.html.twig (replace BLOCKNAME with the block's machine name).

-----------------------------------------------------------------------------------------------------------

He modificat posant un paràgraf HTML a: 
/var/www/hola.com/themes/my_new_theme/templates/layout/html.html.twig
I ho he vist reflectit!!!

Vaig per 'https://www.drupal.org/docs/develop/theming-drupal' (Adding regions to a theme)

