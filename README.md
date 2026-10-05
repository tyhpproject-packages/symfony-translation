<!-- tyhp-readme:start -->
# tyhpdef/symfony-translation

Tyhp type definitions for `symfony/translation` `7.4.17`.

```bash
composer require --dev tyhpdef/symfony-translation:7.4.17
```

This is a metapackage. Composer also installs `tyhpdef/symfony-translation-impl` (type files).
Require **this** name, not `tyhpdef/symfony-translation-impl`.

See https://tyhplang.com.

## Maintain `symfony/translation`? Ship the types yourself

If you are a Packagist maintainer of `symfony/translation`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-translation-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/translation` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-translation": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/translation` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/translation` with a real constraint,
   `"replace": { "tyhpdef/symfony-translation": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/translation` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-translation` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
