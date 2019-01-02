---
layout: default
title: Getting Started
nav_order: 1
permalink: /
---

![Overview]({{ site.baseurl }}/assets/images/overview.png)

# Laravel-powered Finance Tracker and CRM
{: .fs-9 }

Bookkeeper is a flexible finance tracker and CRM powered by [Laravel](https://laravel.com/).  
**Important:** Bookkeeper is still in alpha version and can still receive core changes. Use it at your own risk!
{: .fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/umomega/bookkeeper){: .btn .fs-5 }

---

## Features (very briefly)
- Responsive and easy-to-use UI
- Finance tracking through an overview, accounts, and tags
- Multiple currency support
- Real-time currency rate updates
- CRM for clients, people, and lists
- Pretty installer and updater

## Requirements
Bookkeeper's requirements are the same with [Laravel 5.7 (or higher) requirements](https://laravel.com/docs/5.7#server-requirements).

---

## Getting Started
### Installation
Installing Bookkeeper is fairly simple thanks to it's pretty installer and involves only extracting a ZIP package and creating a database.

![Pretty Installer](/assets/images/install-1.png)

1. **Just download the latest release from [GitHub](https://github.com/umomega/bookkeeper/releases) and extract the package to your server.**  
Since Bookkeeper is structured in the same way of a Laravel application your server's public directory should point to the `public` directory.  
<small>It is possible to change the setting for the public directory inside the `.env` file.</small>
2. **Create a new MySQL database.**  
Bookkeeper will ask for the name, host, port, username, and password for the database during installation.  
![Database Options](/assets/images/install-2.png)  
<small>For other database drivers you will have to configure the `config/database.php`, and `.env` files.
3. **Just run the installer by pointing your browser to the root URL of the setup.**  
Bookkeeper will do the rest.

---

## About the project

Bookkeeper is &copy; 2018 by [umΩ](http://umomega.com).

### License

Bookkeeper is distributed by an [MIT license](https://github.com/umomega/Bookkeeper/blob/master/LICENSE).
