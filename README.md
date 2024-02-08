# Magento 2 Module MgtWizards Auto-Remove Admin Notifications Messages (by shopwhizzy.com)

 - [Main Functionalities](#markdown-header-main-functionalities)
 - [Installation](#markdown-header-installation)
 - [Specifications](#markdown-header-specifications)

## Main Functionalities
Magento 2 admin notifications can be very annoying. This cron will run every hour and remove all unread messages.

## Installation
\* = in production please use the `--keep-generated` option

### Type 1: Zip file

 - Unzip the zip file in `app/code/MgtWizards`
 - Enable the module by running `php bin/magento module:enable MgtWizards_AutoRemoveAdminNotifications`
 - Apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`

### Type 2: Composer

 - Make the module available in a composer repository for example:
    - private repository `repo.magento.com`
    - public repository `packagist.org`
    - public github repository as vcs
 - Add the composer repository to the configuration by running `composer config repositories.repo.magento.com composer https://repo.magento.com/`
 - Install the module composer by running `composer require mgtwizards/module-autoremoveadminnotifications`
 - enable the module by running `php bin/magento module:enable MgtWizards_AutoRemoveAdminNotifications`
 - apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`

## Specifications

 - Cronjob
	- mgtwizards_autoremoveadminnotifications_removeadminmessages

