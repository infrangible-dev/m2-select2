# Infrangible Select2

Provides [Select2](https://select2.org) 4.1.0-rc.0 (MIT license) for other modules: select boxes with search, in the
frontend and in the admin. The module changes nothing in the store on its own.

## Usage

The script is the RequireJS module `Infrangible_Select2/js/select2`, a jQuery plugin:

```javascript
define(['jquery', 'Infrangible_Select2/js/select2'], function ($) {
    $('select.my-select').select2();
});
```

The styles of Select2 are part of the styles of every theme (`view/base/web/css/source/_module.less`).

For example, [Infrangible Catalog Product Option Select2](https://www.infrangible.dev/modules/catalog-product-option-select2)
adds custom options of products with Select2.

## Requirements

- Magento Open Source or Adobe Commerce 2.4.6 or newer
- PHP 8.1 or newer

## Installation

```bash
composer require infrangible/m2-select2
bin/magento module:enable Infrangible_Select2
bin/magento setup:upgrade
```

In production mode, also run `bin/magento setup:static-content:deploy`.

## License

Infrangible Select2 is licensed under the MIT License - see the LICENSE file for details.
