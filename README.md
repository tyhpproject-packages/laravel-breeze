<!-- tyhp-readme:start -->
# tyhpdef/laravel-breeze

Tyhp type definitions for `laravel/breeze` `2.4.2`.

```bash
composer require --dev tyhpdef/laravel-breeze:2.4.2
```

This is a metapackage. Composer also installs `tyhpdef/laravel-breeze-impl` (type files).
Require **this** name, not `tyhpdef/laravel-breeze-impl`.

See https://tyhplang.com.

## Maintain `laravel/breeze`? Ship the types yourself

If you are a Packagist maintainer of `laravel/breeze`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/laravel-breeze-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `laravel/breeze` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/laravel-breeze": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `laravel/breeze` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `laravel/breeze` with a real constraint,
   `"replace": { "tyhpdef/laravel-breeze": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `laravel/breeze` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/laravel-breeze` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
