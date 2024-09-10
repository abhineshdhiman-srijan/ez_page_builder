# ez_page_builder

# Run below commands to install the recipe:

composer create-project drupal/recommended-project:^10.0 MY_PROJECT

cd MY_PROJECT;

composer config repositories.1 vcs <https://github.com/abhineshdhiman-srijan/ezcontent-block>

composer config repositories.2 vcs <https://github.com/abhineshdhiman-srijan/ezcontent-paragraphs>

composer config repositories.3 vcs <https://github.com/abhineshdhiman-srijan/ezcontent-node>

composer config repositories.4 composer <https://github.com/abhineshdhiman-srijan/ez_page_builder>

composer config repositories.5 composer <https://gitlab.ewdev.ca/yonas.legesse/drupal-recipe-unpack.git>

composer config repositories.6 composer <https://asset-packagist.org>

composer config minimum-stability dev

composer config extra.enable-patching true

composer config --no-plugins allow-plugins.cweagans/composer-patches true

composer config --no-plugins allow-plugins.oomphinc/composer-installers-extender true

composer require cweagans/composer-patches

composer require ewcomposer/unpack:dev-master

composer config allow-plugins.ewcomposer/unpack true

composer require drupal_recipe/ez_page_builder:dev-main


# Run below commands to install the recipe using ddev


mkdir my-drupal-project

cd my-drupal-project

ddev config --project-type=drupal9 --docroot=web --create-docroot

ddev start

ddev composer create drupal/recommended-project:^10.1

ddev composer config repositories.1 vcs <https://github.com/abhineshdhiman-srijan/ezcontent-block>

ddev composer config repositories.2 vcs <https://github.com/abhineshdhiman-srijan/ezcontent-paragraphs>

ddev composer config repositories.3 vcs <https://github.com/abhineshdhiman-srijan/ezcontent-node>

ddev composer config repositories.4 composer <https://github.com/abhineshdhiman-srijan/ez_page_builder>

ddev composer config repositories.5 composer <https://gitlab.ewdev.ca/yonas.legesse/drupal-recipe-unpack.git>

ddev composer config repositories.6 composer <https://asset-packagist.org>

ddev composer config minimum-stability dev

ddev composer config extra.enable-patching true

ddev composer config --no-plugins allow-plugins.cweagans/composer-patches true

ddev composer config --no-plugins allow-plugins.oomphinc/composer-installers-extender true

ddev composer require cweagans/composer-patches

ddev composer require ewcomposer/unpack:dev-master

ddev composer config allow-plugins.ewcomposer/unpack true

ddev composer require drupal_recipe/ez_page_builder:dev-main

ddev composer require drush/drush
ddev drush si
ddev drush recipe recipes/custom/ez_page_builder;
