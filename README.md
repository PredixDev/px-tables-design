# Tables

Predix Experience has some useful helpers for common `<table>` patterns. This module is a fork of the [inuitcss Table module](https://github.com/inuitcss/objects.tables).

## Dependencies

Px's Tables module depends on three other Px and inuitcss modules:

* [px-defaults-design](https://github.sw.ge.com/PXd/px-defaults-design)
* [px-functions-design](https://github.sw.ge.com/PXd/px-functions-design)
* [px-normalize-design](https://github.sw.ge.com/PXd/px-normalize-design)

## Installation

Install this module and its dependencies using bower:

    bower install --save https://github.sw.ge.com/PXd/px-tables-design.git

Once installed, `@import` into your project's Sass file in its Objects layer:

    @import "../px-tables-design/objects.tables";

See [px-getting-started](https://github.sw.ge.com/PXd/px-getting-started#a-note-about-relative-import-paths) for an explanation of the `../`

## Import once

All rulesets are wrapped in the following `@if` statement:

    @if import-once('objects.tables') { ... }

## Usage

These flags are available and, if needed, should be set to `true` prior to importing the module:

    $inuit-enable-table--fixed
    $inuit-enable-table--compact
    $inuit-enable-table--cosy
    $inuit-enable-table--comfy
    $inuit-enable-table--cells
    $inuit-enable-table--rows
    $inuit-enable-table--columns

The following variables are available for use in the module:

    $inuit-table-border-width
    $inuit-table-border-style
    $inuit-table-border-color

The following dimension (padding) variables can be customized:

    $inuit-table-padding--compact
    $inuit-table-padding--cosy
    $inuit-table-padding--comfy

## Options

These classes are available if the variable flags listed above are set to `true`:

* `table--fixed`: force tables into having equal-width columns.
* `table--compact`: tables with very tightly packed cells.
* `table--cosy`: tables with lightly packed cells.
* `table--comfy`: tables with very widely padded cells.
* `table--cells`: add borders around a `table`.
* `table--rows`: add borders only to `table`’s rows.
* `table--columns`: add borders only to `table`’s columns.
