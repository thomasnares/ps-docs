---
title: Products lifecycle
weight: 42
useMermaid: true
---

# Products lifecycle


## Product visibility

## Product indexing

Product indexing is triggered by :

- Search::indexation(true) // full update

- Search::indexation(false, $productId) // only one product

Search::indexation(true) is triggered by : 

- controllers/admin/AdminShopController.php
- src/PrestaShopBundle/Install.php
- controllers/admin/AdminSearchController.php

