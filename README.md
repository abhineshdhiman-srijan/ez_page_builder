
# drupal_recipe/ez_page_builder

Provides Landing Page Builder with components


## Installation

#### Install the project using composer 

```bash
composer create-project drupal/recommended-project:^10.0 MY_PROJECT
cd MY_PROJECT;
composer config repositories.ezcontent-block vcs https://github.com/abhineshdhiman-srijan/ezcontent-block
composer config repositories.ezcontent-paragraphs vcs https://github.com/abhineshdhiman-srijan/ezcontent-paragraphs
composer config repositories.ezcontent-node vcs https://github.com/abhineshdhiman-srijan/ezcontent-node
composer config repositories.ez_page_builder vcs https://github.com/abhineshdhiman-srijan/ez_page_builder
composer config repositories.drupal8 composer https://packages.drupal.org/8
composer config repositories.asset-packagist composer https://asset-packagist.org
composer config minimum-stability dev
composer config extra.enable-patching true
composer config --no-plugins allow-plugins.cweagans/composer-patches true
composer config --no-plugins allow-plugins.oomphinc/composer-installers-extender true
composer require cweagans/composer-patches
composer require ewcomposer/unpack:dev-master
composer config allow-plugins.ewcomposer/unpack true
composer require drupal_recipe/ez_page_builder:dev-main
```
#### ddev setup

```bash
composer create-project drupal/recommended-project:^10.0 MY_PROJECT
cd MY_PROJECT;
composer config repositories.1 vcs https://github.com/abhineshdhiman-srijan/ezcontent-block
composer config repositories.2 vcs https://github.com/abhineshdhiman-srijan/ezcontent-paragraphs
composer config repositories.3 vcs https://github.com/abhineshdhiman-srijan/ezcontent-node
composer config repositories.4 vcs https://github.com/abhineshdhiman-srijan/ez_page_builder
composer config repositories.5 composer https://gitlab.ewdev.ca/yonas.legesse/drupal-recipe-unpack.git
composer config repositories.6 composer https://asset-packagist.org
composer config minimum-stability dev
composer config extra.enable-patching true
composer config --no-plugins allow-plugins.cweagans/composer-patches true
composer config --no-plugins allow-plugins.oomphinc/composer-installers-extender true
composer require cweagans/composer-patches
composer require ewcomposer/unpack:dev-master
composer config allow-plugins.ewcomposer/unpack true
composer require drupal_recipe/ez_page_builder:dev-main
```
## Tech Stack

**CMS:** Drupal


