<!-- tyhp-readme:start -->
# tyhpdef/phpstan-phpdoc-parser

Tyhp type definitions for `phpstan/phpdoc-parser` `2.3.5`.

```bash
composer require --dev tyhpdef/phpstan-phpdoc-parser:2.3.5
```

This is a metapackage. Composer also installs `tyhpdef/phpstan-phpdoc-parser-impl` (type files).
Require **this** name, not `tyhpdef/phpstan-phpdoc-parser-impl`.

See https://tyhplang.com.

## Maintain `phpstan/phpdoc-parser`? Ship the types yourself

If you are a Packagist maintainer of `phpstan/phpdoc-parser`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/phpstan-phpdoc-parser-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `phpstan/phpdoc-parser` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/phpstan-phpdoc-parser": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `phpstan/phpdoc-parser` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `phpstan/phpdoc-parser` with a real constraint,
   `"replace": { "tyhpdef/phpstan-phpdoc-parser": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `phpstan/phpdoc-parser` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/phpstan-phpdoc-parser` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
