JohannesSteu.Neos.FlexBoxGrid
=================================

This is a package based on [JohannesSteu.Bootstrap.GridSystem](https://github.com/johannessteu/JohannesSteu.Bootstrap.GridSystem) and implements a grid system based on a flexbox approach.
This Package also bundles stylesheets and uses therefore [flexboxgrid](https://github.com/kristoferjoseph/flexboxgrid) / http://flexboxgrid.com/


Installation
------------
Just install it via composer
```
composer require johannessteu/neos-flexboxgrid
```
or just copy this package in YOUR_ROOT/Applications/JohannesSteu.Neos.FlexBoxGrid

Afterwards the Root.ts2 will be auto-included in your main TypoScript. Otherwise use
```
include: resource://JohannesSteu.Neos.FlexBoxGrid/Private/TypoScript/Root.ts2
```
in your Root.ts2.

Inside your Template you need to include the stylesheets:
```
<link rel="stylesheet" type="text/css" href="{f:uri.resource(package: 'JohannesSteu.Neos.FlexBoxGrid', path: 'Styles/flexboxgrid.min.css')}" media="all">
```
inside your head-Section. You could also include in your distribution the npm module `flexboxgrid` and use those files.

Usage
-----
To use this plugin just create a new ContentElement inside your page and choose one of the new types. The Inspector-Pane will give you access to all different layouts and settings.
For further informations about usage check [JohannesSteu.Bootstrap.GridSystem](https://github.com/johannessteu/JohannesSteu.Bootstrap.GridSystem)