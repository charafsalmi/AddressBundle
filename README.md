[![SensioLabsInsight](https://insight.sensiolabs.com/projects/18a3a11d-2510-44ff-8c9e-b5d2902adde7/mini.png)](https://insight.sensiolabs.com/projects/18a3a11d-2510-44ff-8c9e-b5d2902adde7)

HADONRA - address-bundle
========================

If you want to set an address to yours entities (user, place or other), use this bundle.

1) Installation
---------------

Add to composer and update.

```
"require": {
    "hadonra/address-bundle": "dev-master"
}
```

2) Define your bazinga geocoder provider
----------------------------------------

Must configure bazinga geocoder both.

```
# app/config/config.yml
hadonra_address:
    provider:   google_maps
```

3) Dump Countries, Region, Department and city
----------------------------------------------

In order to have geoloc data, use this command :

```
php app/console hadonra:address:load-fixture --append
```



