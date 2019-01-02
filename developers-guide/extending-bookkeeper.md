---
layout: default
title: Extending Bookkeeper
parent: Developer's Guide
nav_order: 2
permalink: /developers-guide/extending-bookkeeper
---

# Extending Bookkeeper
{:.no_toc}

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

There are two main ways to extend Bookkeeper: The Extension Directory and Themes
{: .fs-6 .fw-300 }

## Extensions
The main location to add new functionality is under the `extension` directory as it is auto-loaded by composer.
```js
...
"autoload": {
    "classmap": [
        "database/seeds",
        "database/factories"
    ],
    "psr-4": {
        "Bookkeeper\\": "app/",
        "Extension\\": "extension/"
    }
},
...
```
The rest is the same as adding new packages to Laravel. Please check [Service Providers](https://laravel.com/docs/5.7/providers) and [Package Development](https://laravel.com/docs/5.7/packages).

## Themes
Bookkeeper uses the `igaster/laravel-theme` package for managing views and assets. Please check the [Documentation](https://github.com/igaster/laravel-theme/wiki/1.-Installation) to learn how to extend the UI in Bookeeper.
