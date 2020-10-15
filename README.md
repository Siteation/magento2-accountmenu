# Siteation - Magento 2 Account Menu

[![Packagist Version](https://img.shields.io/packagist/v/siteation/magento2-module-account-menu)](https://packagist.org/packages/siteation/magento2-module-account-menu)

This module adds an account menu next to the minicart.
So that you can access account menu more easily.

This module works similar to the Luma theme account menu.
Where it takes the top.links and adds them to a dropdown.

The only exception is that this menu does not move the top.links.
But instead renders new account menu with the same links, from top.links.
And also adds extra menu items.
That are also found in the account dashboard menu.
For a quicker navigation.

If you are planing to use this menu instead of the top.links.
See the wiki on how to do this.

## Installation

Install the package via;

```bash
composer require siteation/magento2-module-account-menu
bin/magento setup:upgrade
```

> This Module require Magento 2.3 or higher!
> For more requirements see the `composer.json`.

## How to use

Not instructions needed.
This module works out of the box for themes based on Luma theme.

If you use the Blank theme instead.
Make sure add `@account-menu-theme: "blank";` to your own theme.
To load the Blank theme styles instead of Luma.

### SCSS support

This module also supports SCSS styles that can be used with tools like [Frontools](https://github.com/SnowdogApps/magento2-frontools).

Add `Siteation_AccountMenu` to the themes.json;

```json
{
    "<THEME>": {
        "modules": {
            "Siteation_AccountMenu": "vendor/siteation/magento2-module-account-menu/view/frontend"
        }
    }
}
```

And import it in your `styles.scss` via;

```scss
@import "../Siteation_AccountMenu/styles/module";
```

## Tips

The wiki is full of nice theming options.
And tricks with this menu and themes.
So check out the wiki.
