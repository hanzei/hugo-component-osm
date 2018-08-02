# OpenStreetMap shortcode for hugo
[![Build Status](https://travis-ci.com/Hanzei/hugo-component-osm.svg?branch=master)](https://travis-ci.com/Hanzei/hugo-component-osm)

## Getting started

Run from the root of your Hugo site:
```sh
$ git clone https://github.com/Hanzei/hugo-component-osm.git themes/osm
```

Alternatively you can include this repository as a [git submodule](https://git-scm.com/book/de/v1/Git-Tools-Submodule). This makes it easier to update this theme if you have your Hugo site in git as well. For this you need to run:

```sh
$ git submodule add https://github.com/Hanzei/hugo-component-osm.git themes/osm
```

Now you just have to add this theme component to your themes in `config.toml`, e.g. `theme = ["osm", "base-theme"]`. See the [Hugo documentation](https://gohugo.io/themes/theme-components/) for more infos.

## Creating and including a map

First create a map for free on https://umap.openstreetmap.fr/en/. Then include this map by using the `openstreetmap` shortcode, e.g. `{{< openstreetmap mapName="demo-map_1" >}}`

## Options

The only required parameter is `mapName`. All other parameters are completely optional.

Available parameter are:
- `coordX` (default `auto`)
- `coordY` (default `auto`)
- `scale`  (default `auto`)
- `scaleControl` (default `true`)
- `miniMap` (default `false`)
- `scrollWheelZoom` (default `true`)
- `zoomControl` (default `true`)
- `allowEdit` (default `false`)
- `moreControl` (default `true`)
- `searchControl` (default `true`)
- `tilelayersControl` (default `null`)
- `embedControl` (default `null`)
- `datalayersControl` (default `true`)
- `onLoadPanel` (default `none`)
- `captionBar` (default `true`)
