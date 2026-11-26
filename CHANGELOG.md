# Changelog

## 2.0.1

### Changed

- Supports PHP 8.1 again, like Magento 2.4.6: the Adobe Commerce Marketplace requires modules to allow every PHP
  version of the Magento versions they support.

## 2.0.0

### Breaking changes

- Requires Magento 2.4.6 or newer and PHP 8.2 or newer. Magento 2.4.4 and 2.4.5 and PHP 7.1 to 8.1 are no longer
  supported; use version 1.x for these.
- Requires `infrangible/m2-foundation` 3.0; no longer requires `fewedev/xml`, which the module does not use.

### Changed

- The module is loaded after Infrangible Foundation.
- The script and the stylesheet of Select2 are excluded from the Magento coding standard, they stay as released.
- Rules that the themes default and classic of Select2 share are LESS mixins; the compiled CSS has the same rules.
- README.
- Checks with PHPStan level 9 and the Magento coding standard on every push.
