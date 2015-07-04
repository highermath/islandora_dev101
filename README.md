This 2-hour workshop will introduce Islandora objects and how they work within Drupal. It will also cover the basics of Islandora modules, and introduce Drupal hooks. The workshop doesn't cover Solr indexing, Drupal theming, writing tests for Islandora modules or access control in Islandora.

In the second hour of the workshop, participants will start coding their own simple Islandora module. To prepare for this part of the workshop, make sure you have installed the [Islandora Vagrant](https://github.com/Islandora-Labs/islandora_vagrant) virtual machine on your laptop.

## Outline

* Islandora objects
* Islandora's relationship with Drupal
* Tuque
* Islandora modules
  * Types: solution packs, integration modules utility modules
  * Structure
  * Islandora coding conventions
  * Islandora API
  * Hooks

## Islandora objects
Are fundamentally Fedora objects. Content models, structure/properties

## Islandora's relationship with Drupal


## Tuque


## Islandora modules

### Types

### Structure

Simplest:

```
.
├── islandora_foo.info
├── islandora_foo.module
├── LICENSE
├── README.md
```

Average complexity:
```
.
├── build
│   └── Doxyfile
├── build.xml
├── css
│   └── islandora_fits.css
├── includes
│   ├── admin.form.inc
│   └── derivatives.inc
├── islandora_fits.info
├── islandora_fits.install
├── islandora_fits.module
├── LICENSE.txt
├── README.md
└── theme
    └── islandora-fits-metadata.tpl.php
```

Hi complexity:

```
.
├── build
│   └── Doxyfile
├── build.xml
├── css
│   └── islandora_book.css
├── data
│   ├── datastreams
│   │   ├── islandora_bookCModel_ds_composite_model.xml
│   │   └── islandora_book_collection_policy.xml
│   └── forms
│       └── book_form_mods.xml
├── images
│   └── folder.png
├── includes
│   ├── admin.form.inc
│   └── manage_book.inc
├── islandora_book.info
├── islandora_book.install
├── islandora_book.module
├── LICENSE.txt
├── README.md
├── tests
│   ├── fixtures
│   │   └── test.tiff
│   ├── islandora_book_derivatives_ingest_purge.test
│   ├── islandora_book_ingest_purge.test
│   └── scripts
│       ├── adore.sh
│       └── tesseract.sh
└── theme
    ├── islandora-book-book.tpl.php
    ├── islandora-book-page-img-print.tpl.php
    ├── islandora-book-page.tpl.php
    └── theme.inc
```

### Islandora coding conventions


### Islandora API


### Hooks

[Islandora provides many](https://github.com/Islandora/islandora/blob/7.x/islandora.api.php). In this workshop, we'll focus on the ones that are fired during the object add/update/purge lifecycle, and use a couple of others.

