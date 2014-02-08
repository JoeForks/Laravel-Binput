Laravel Binput
==============


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/GrahamCampbell/Laravel-Binput/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
[![Build Status](https://travis-ci.org/GrahamCampbell/Laravel-Binput.png)](https://travis-ci.org/GrahamCampbell/Laravel-Binput)
[![Coverage Status](https://coveralls.io/repos/GrahamCampbell/Laravel-Binput/badge.png)](https://coveralls.io/r/GrahamCampbell/Laravel-Binput)
[![Scrutinizer Quality Score](https://scrutinizer-ci.com/g/GrahamCampbell/Laravel-Binput/badges/quality-score.png?s=5b1bca08ae3b2c0cdfc2be27541d5dd077e03200)](https://scrutinizer-ci.com/g/GrahamCampbell/Laravel-Binput)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/eb11c61f-b689-4453-8d68-08a68861e6d5/mini.png)](https://insight.sensiolabs.com/projects/eb11c61f-b689-4453-8d68-08a68861e6d5)
[![Software License](https://poser.pugx.org/graham-campbell/binput/license.png)](https://github.com/GrahamCampbell/Laravel-Binput/blob/master/LICENSE.md)
[![Latest Version](https://poser.pugx.org/graham-campbell/binput/v/stable.png)](https://packagist.org/packages/graham-campbell/binput)


## What Is Laravel Binput?

Laravel Binput is an input protector for [Laravel 4.1](http://laravel.com).

* Laravel Binput was created by, and is maintained by [Graham Campbell](https://github.com/GrahamCampbell).
* Laravel Binput relies on my [Laravel Security](https://github.com/GrahamCampbell/Laravel-Security) package.
* Laravel Binput uses [Travis CI](https://travis-ci.org/GrahamCampbell/Laravel-Binput) with [Coveralls](https://coveralls.io/r/GrahamCampbell/Laravel-Binput) to check everything is working.
* Laravel Binput uses [Scrutinizer CI](https://scrutinizer-ci.com/g/GrahamCampbell/Laravel-Binput) and [SensioLabsInsight](https://insight.sensiolabs.com/projects/eb11c61f-b689-4453-8d68-08a68861e6d5) to run additional checks.
* Laravel Binput uses [Composer](https://getcomposer.org) to load and manage dependencies.
* Laravel Binput provides a [change log](https://github.com/GrahamCampbell/Laravel-Binput/blob/master/CHANGELOG.md), [releases](https://github.com/GrahamCampbell/Laravel-Binput/releases), and [api docs](http://grahamcampbell.github.io/Laravel-Binput).
* Laravel Binput is licensed under the Apache License, available [here](https://github.com/GrahamCampbell/Laravel-Binput/blob/master/LICENSE.md).


## System Requirements

* PHP 5.4.7+ or PHP 5.5+ is required.
* You will need [Laravel 4.1](http://laravel.com) because this package is designed for it.
* You will need [Composer](https://getcomposer.org) installed to load the dependencies of Laravel Binput.


## Installation

Please check the system requirements before installing Laravel Binput.

To get the latest version of Laravel Binput, simply require `"graham-campbell/binput": "1.0.*@beta"` in your `composer.json` file. You'll then need to run `composer install` or `composer update` to download it and have the autoloader updated.

You will need to register the [Laravel Security](https://github.com/GrahamCampbell/Laravel-Security) service provider before you attempt to load the Laravel Binput service provider. Open up `app/config/app.php` and add the following to the `providers` key.

* `'GrahamCampbell\Security\SecurityServiceProvider'`

Once Laravel Binput is installed, you need to register the service provider. Open up `app/config/app.php` and add the following to the `providers` key.

* `'GrahamCampbell\Binput\BinputServiceProvider'`

You can register the Binput facade in the `aliases` key of your `app/config/app.php` file if you like.

* `'Binput' => 'GrahamCampbell\Binput\Facades\Binput'`


## Configuration

Laravel Binput requires no configuration. Just follow the simple install instructions and go!


## Usage

There is currently no usage documentation besides the [API Documentation](http://grahamcampbell.github.io/Laravel-Binput
) for Laravel Binput.

You may see an example of implementation in [CMS Core](https://github.com/GrahamCampbell/CMS-Core).


## Updating Your Fork

Before submitting a pull request, you should ensure that your fork is up to date.

You may fork Laravel Binput:

    git remote add upstream git://github.com/GrahamCampbell/Laravel-Binput.git

The first command is only necessary the first time. If you have issues merging, you will need to get a merge tool such as [P4Merge](http://perforce.com/product/components/perforce_visual_merge_and_diff_tools).

You can then update the branch:

    git pull --rebase upstream master
    git push --force origin <branch_name>

Once it is set up, run `git mergetool`. Once all conflicts are fixed, run `git rebase --continue`, and `git push --force origin <branch_name>`.


## Pull Requests

Please review these guidelines before submitting any pull requests.

* When submitting bug fixes, check if a maintenance branch exists for an older series, then pull against that older branch if the bug is present in it.
* Before sending a pull request for a new feature, you should first create an issue with [Proposal] in the title.
* Please follow the [PSR-2 Coding Style](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md) and [PHP-FIG Naming Conventions](https://github.com/php-fig/fig-standards/blob/master/bylaws/002-psr-naming-conventions.md).


## License

Apache License

Copyright 2013-2014 Graham Campbell

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
