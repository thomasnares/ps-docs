---
title: "Module use-case : Customer Pet List"
weight: 30
aliases:
  - /1.7/modules/pet-list/
---

Use Case : Customer Pet List
===============

In this use-case, we will create a new entity representing Pets (animals), that we will attach to Customers (n,1 relation to Pets). 

We will learn how to create a CRUD in backoffice to allow administration of this entity.

For this use-case, we will use ObjectModel (note that Prestashop now uses CQRS pattern, read more here : /1.7/development/architecture/domain/cqrs/#why-using-cqrs-in-prestashop)

## Summary

- Basic module initialization
- ObjectModel creation
- FormDataProvider and FormDataHandler
- Creating the Grid


{{% children %}}