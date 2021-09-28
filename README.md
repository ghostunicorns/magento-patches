# Install

Install Composer Patches (https://github.com/cweagans/composer-patches)

`composer require cweagans/composer-patches`

# Configure

Inside your `composer.json` add the patches for the desidered module, specifying a custom message and the patch path.

```
{
...
  "extra": {
    "patches": {
      "magento/module-cron": {
        "Fix the app:config:import Magento Cron Config error": "m2-hotfixes/magento-module-cron-config-product-alert.patch"
      },
      "paypal/module-braintree-core": {
          "Fix app:config:import error": "m2-hotfixes/magento-paypal-braintree-config-array.patch"
      }
    }
  }
...
}
```

# Apply

`composer install`

# Contribution

Yes, of course you can contribute sending a pull request to propose improvements and fixes.

