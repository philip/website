+++
title = "Commands"
description = "BookStack command-line actions"
date = "2017-02-26"
type = "admin-docs"
+++

BookStack has some command line actions that can help with maintenance and common operations. There are also many commands available from the underlying Laravel framework. To list all available commands you can simply run `php artisan` from your BookStack install folder. Custom BookStack commands are all under the 'bookstack' namespace.

### BookStack Commands

Here's a listing of the BookStack specific commands:

```bash

# Delete all activity history from the system
php artisan bookstack:clear-activity

# Delete all page revisions from the system
php artisan bookstack:clear-revisions

# Delete all page revisions from the system including update drafts
php artisan bookstack:clear-revisions -a

# Delete all page views from the system
php artisan bookstack:clear-views

# Generate SQL commands that will upgrade the database to UTF8mb4
# See https://www.bookstackapp.com/docs/admin/ut8mb4-support/
php artisan bookstack:db-utf8mb4

# Rebuild the search index
# Useful if manually inserting pages into the system
php artisan bookstack:regenerate-search

# Regenerate access permissions - Used mostly in development
php artisan bookstack:regenerate-permissions

```
