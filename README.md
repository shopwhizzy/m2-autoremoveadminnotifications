# Magento 2 Module ShopWhizzy Auto-Remove Admin Notifications Messages (by shopwhizzy.com)

 - [Main Functionalities](#markdown-header-main-functionalities)
 - [Installation](#markdown-header-installation)
 - [Specifications](#markdown-header-specifications)
 - [Copyright](#markdown-header-copyright)

## Main Functionalities
Magento 2 admin notifications can be very annoying. This cron will run every hour and remove all unread messages.

## Installation
\* = in production please use the `--keep-generated` option

### Type 1: Zip file

 - Unzip the zip file in `app/code/ShopWhizzy/AutoRemoveAdminNotifications`
 - Enable the module by running `php bin/magento module:enable ShopWhizzy_AutoRemoveAdminNotifications`
 - Apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`

 ### Type 2: Composer

- Install using [Composer](https://getcomposer.org).

```
composer require shopwhizzy/module-autoremoveadminnotifications
php bin/magento module:enable ShopWhizzy_AutoRemoveAdminNotifications
php bin/magento setup:upgrade
```

## Specifications

 - Cronjob
	- shopwhizzy_autoremoveadminnotifications_removeadminmessages

## Copyright

 - developed by [ShopWhizzy.com](https://shopwhizzy.com/magento)

