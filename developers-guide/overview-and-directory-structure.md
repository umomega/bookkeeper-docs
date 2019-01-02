---
layout: default
title: Overview and Directory Structure
parent: Developer's Guide
nav_order: 1
permalink: /developers-guide/overview-and-directory-structure
---

# Overview and Directory Structure
{:.no_toc}

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

Since Bookkeeper is a Laravel app the directory structure is almost the same with any Laravel app with some minor additions. Consequently, you can do everything that you can do with a Laravel application.
{: .fs-6 .fw-300 }

## Directory Structure
Bookkeeper has an auto-updater which updates some directories and files with new releases. If you edit the contents of the directories that are marked as `not-editable` below you might break Bookkeeper and the changes you made will be overwritten with the next update. All other directories can be modified and can have new functionality added just like a standard Laravel app.

```
+-- app (not-editable)
|-- bootstrap (not-editable)
|-- config (editable)
|-- database (not-editable)
|-- extension (editable)
|-- public (editable)
|   |-- assets (editable)
|   |   +-- bookkeeper (not-editable)
|   |
|-- resources (editable)
|   |-- js (not-editable)
|   |-- lang (not-editable)
|   |-- sass (not-editable)
|   |-- views (editable)
|   |   |-- install (not-editable)
|   |   +-- bookkeeper (not-editable)
|   |
|-- routes (editable)
|-- |   +-- bookkeeper (not-editable)
|   |
|-- storage (editable)
|-- tests (editable)
|-- vendor (not-editable)
|
|-- artisan (not-editable)
|-- composer.json (not-editable)
|-- (Other Laravel Files) (not-editable)
+-- ..
```
The main location to add new functionality is under the `extension` directory as it is auto-loaded by composer. For more information about Extending Bookkeeper please check the next chapter.

## App Directory
The `app` directory contains the core functionality for Bookkeeper. There is no separate API documentation for this but the code is well documented inside.
```
+-- Console: Standard Laravel Console Kernel
|-- CRM: Contains models for the CRM functionality
|-- Exceptions: Standard Laravel Exception Handler
|-- Exports: Contains Exporters
|-- Finance: Contains models for the Finance functionality
|-- Html: Contains HTML generators
|-- Http: Contains the controllers, middleware and requests as well as the Http Kernel just like a standard Laravel app
|-- Notifications: Standart Laravel Notifications Namespace
|-- Observers: Contains observers for various models and their model events
|-- Providers: Contains the service providers just like a standard Laravel app
|-- Support: Contains support services, helpers and snippets
+-- Users: Contains the models for Users
```
