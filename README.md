# Docker PHP Quality Tools for Drupal8 project.

Docker image for running:

* [PHP QA Tools](https://edgedesigncz.github.io/phpqa/)
* [PHPloc](https://github.com/sebastianbergmann/phploc)
* [Count Lines of Code (cloc)](https://github.com/AlDanial/cloc)

# Examples

**phpqa**

    docker run --rm -u $UID -v $PWD:/app lucacracco/phpqa-drupal phpqa --report --ignoredDirs vendor,node_modules --analyzedDirs web/modules/custom

**phploc**

    docker run --rm -u $UID -v $PWD:/app lucacracco/phpqa-drupal phploc web/modules/custom

**cloc**

    docker run --rm -u $UID -v $PWD:/app lucacracco/phpqa-drupal cloc web/modules/custom