# Domain Menu (D7)

## About
This module provides ability to administer menus per domain, in a similar way to what
domain_access does to nodes.

This is a Drupal 7 back-port of the Drupal 8 version of the
[Domain Menu](https://www.drupal.org/project/domain_menu) module. There is an
[open issue](https://www.drupal.org/project/domain_menu/issues/2965629) to have this repository
merged to 7.x-1.x branch of the original module.

## Provided Permission compared to menu permissions
The Provided permission is largely inspired by domain_access and what it makes possible for
nodes (except for that menus don't have bundles, so mapping isn't exactly 1:1 with nodes).

#### Administer Menus - provided from core's `menu` module.
Allows user to edit, add, delete any menu site-wide regardless of their assigned domain(s)
and regardless of the menus domain(s). In an sense it's like "edit any content" permission.

#### Administer menus and menu items on assigned domains - provided by `domain_menu` module.
Allows a user to edit menus assigned to their relevant domains. Allows full CRUD on menu items
belonging to those menus. Users with the permission cannot delete those menus or create new
menus. This is in a sense like "edit any content on assigned domains" from domain access module.

## Reporting issues
Any issues against this version for Drupal 7 should be reported in GitHib. Once the code is
merged, the Drupal org issue queues should be used.
