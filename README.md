# Asdoria Sylius Demo

<p>
    <img align="left" src="documentation/asdoria-logo.png" width="80" alt="">
</p>

Asdoria is a French company specialized in the design of e-commerce solutions. On a daily basis, we use Sylius for our products and we share some of our work freely. If you think that some of the Sylius plugins we have developed are of interest to you, it is possible to try them via the corresponding demo page below.
If you want to see code of each plugin, check the following link: https://github.com/asdoria

To learn more about us, please visit https://www.asdoria-web-agency.com/

## Table of Content
***

* [**Overview**](#overview)
* [**Available Plugins**](#available-plugins)
    * [Customers Group](#customers-group)
    * [Documents for products](#documents-for-products)
    * [Facet filters](#facet-filters)
    * [Pictograms for products](#pictograms-for-products)
    * [Products comparator](#products-comparator)
    * [Quick Shopping](#quick-shopping)
    * [Retailers Map](#retailers-map)
* [**Demo**](#demo)
* [**Local installation (if wanted)**](#local-installation-if-wanted)
* [**License**](#license)
* [**Contact**](#contact)
***

## Overview
***

Most of e-commerce websites need some additional features to improve user experience or to manage the content of the store in a better way. Indeed, you can choose to **add pictograms or documents** on your products to help your clients to find easily some information, or just **show a map of retailers**. We also provide a **facet filters system** and the possibility to **manage users access (visiblity) to your products**. This page is dedicated to online demonstration of these fonctionnalities but you can install each plugins by following the instructions on their GitHub page, or just read [here](#local-installation-if-wanted) if you want to try all of your work.

## Available plugins
***
* ### Customers Group <img src="documentation/visibility.png" width="32" alt="" style="vertical-align: middle">

  This plugin allow you to manage user access to products. To be more precise, you can define if a user can see a product in your catalog by creating `Customer Groups` that will be used to filter which products are visible for members of this group.

* ### Documents for products <img src="documentation/documents.png" width="32" alt="" style="vertical-align: middle">

  The possibility to associate a product with documents is useful in many cases:

    * give a warranty to the customer,
    * provide a user manual,
    * a detailed size guide if it is a clothing item,
    * etc.

* ### Facet filters <img src="documentation/filters.png" width="32" alt="" style="vertical-align: middle">

  The system of facet filters exists on many famous websites. But Sylius doesn't offer this possibility natively. By using our plugin, you can enhance customer experience on your online store by a ergonomic and efficient filtering system.

* ### Pictograms for products <img src="documentation/pictograms.png" width="32" alt="" style="vertical-align: middle">

  Find easily redudant information can be easily achieved by using a system of pictograms in the description of your products.

* ### Products comparator <img src="documentation/comparator.png" width="32" alt="" style="vertical-align: middle">

  Give the user the ability to compare your products easily with a beautiful integration.

* ### Quick Shopping <img src="documentation/quickshopping.png" width="32" alt="" style="vertical-align: middle">

  Add the possibility to users to add multiple variants in their shopping cart.

* ### Retailers Map <img src="documentation/map.png" width="32" alt="" style="vertical-align: middle">

  You can create retailers group, and retailers with a precise position on the map. Of course, each retailers group can have an icon (like brand's logo) and contact information that will displayed on the map if the user click on the icon. A search bar is also provided in the plugin. Many of the plugin use VueJS with Leaflet.

## Demo
***
Most of our plugin is open source and had an online page to try it. You will find GitHub repository and the online demo link associated to each plugin in the table below.
> **Login:** asdoria \
> **Password:** asdoria

| Asdoria's Plugin                                                         | GitHub                                                      | Online Demo                                                                                                              |
|--------------------------------------------------------------------------|-------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|
| Customers Group                                                          | https://github.com/asdoria/AsdoriaSyliusProductCustomerGroup |                                                              |
| Documents for products                                                   | https://github.com/asdoria/AsdoriaSyliusProductDocumentPlugin |                                                               |
| Facet filters |  https://github.com/asdoria/AsdoriaSyliusFacetFilterPlugin  |                                                                |
| Pictograms for products | https://github.com/asdoria/AsdoriaSyliusPictogramPlugin |                                                             |
| Products comparator | https://github.com/asdoria/AsdoriaSyliusProductComparatorPlugin |                                                                              |
| Quick Shopping | https://github.com/asdoria/AsdoriaSyliusQuickShoppingPlugin |                                                                |
| Retailers Map | https://github.com/asdoria/AsdoriaSyliusRetailerPlugin |  |

## Local installation (if wanted)
***

1. Create a Sylius project:
```
composer create-project sylius/sylius-standard asdoria-demo
cd asdoria-demo

```

2. Install dependencies and initialize database:
```
composer install --no-scripts
php bin/console do:da:cr
composer run post-install-cmd
```

3. Run fixtures:
```
php bin/console doctrine:fixtures:load -q
```
4. Connect:
> **Login:** asdoria \
> **Password:** asdoria

## License
***

All of these plugins source code is completely free.

## Contact
***

The best way to contact us is to contact us by mail at `contact@asdoria.com`.
