---
date: 2017-09-27T10:00:00+06:00
lastmod: 2018-05-24T02:10:00+06:00
title: Seguros ramo "não vida"

categories:
  - features
tags:
  - menus
slug: menus
toc: true
menu:
  sidebar:
    name: seguros não vida
    parent: docs
---
Minimo has three menus.

 +++
1. Main Menu
2. Sidebar Menu
3. Social Menu

## Main Menu

**name**: `main`

Main menu is located at the top of the site.

Check [Hugo's Menus Documentation](https://gohugo.io/content-management/menus/) for information about managing this menu.

You can hide the Main Menu using the following option in your `config.toml` file:

```toml
[params.settings]
hideMainMenu = true
```

## Sidebar Menu

**name**: `sidebar`


You can use Sidebar Menu as normal [Hugo Menus](https://gohugo.io/content-management/menus/).



```toml
[sidebar_menu]
...
mirror = "main"
```

The sidebar menu can display nested menus. The sub-pages need to have a page as `parent` defined in the page's front matter:

```yaml
menu:
   main:
      parent: myParentPage
```

## Social Menu



Use the variables under `[params.social]` in your `config.toml` file for adding your social profiles:

```toml
[params.social]
codepen = "..."
email = "..."
facebook = "..."
...
```

You only have to add your usernames. Minimo will take care of the rest.

#### Changing Social Menu Icons Order



The social menu icons will appear in the order you specify in the `platforms` array.
