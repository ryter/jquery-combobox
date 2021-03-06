#jQuery Combobox plugin

Yet another combobox plugin. Were developed for my own purposes and successfully used in many projects.

##Features

* works with jQuery 1.3.2+

##Usage

Basic usage:

    $('select').combobox([{options}], [{classes}]);

##Parameters

###Options

####`width` and `height`

`int` Determines the `width`/`height` of the element. Defaults is `false` - `width`/`height` will depend on the `width`/`height` of the source element. 

####`btnWidth`

`int` Determines the element's button width (in px). Defaults is 15.

####`showSpeed` and `hideSpeed`

`mixed` Speed of the show/hide animation effect. Defaults is `fast`.

####`hideSelected`

`bool` If is `true` the selected element will he hidden from the dropdown list. By default is `false`.

####`listMaxHeight`

`int` Maximum height of the dropdown list. Vertical scrollbar appears when list height is greater than this value. Defaults is `false` - no limit.

####`hoverEnabled`

`bool` Enables hover feature. For performance reasons by default is `false`

####`theme`

`string` Set the "theme" prefix - it will be used in CSS classes for generated elements. Defaults is `combo`

###Classes

List of default element's CSS classes suffixes and their default values.

* `wrapper` - `wrapper`
* `focus` - `focus`
* `disabled` - `disabled`
* `multiple` - `multiple`
* `button` - `button`
* `group` - `group`
* `groupLabel` - `group-label`
* `list` - `list`
* `selected` - `selected`
* `itemHover` - `item-hover`
* `itemActive` - `item-active` 
* `wrapHover` - `wrapper-hover`
* `wrapActive` - `wrapper-active`
* `listLong` - `list-long`

The applyed css classes will be prepared from `theme_name-suffix_name`

##Events

You can bind several event handlers to the source (select) element, to catch some usefull events.

###`before_show` and `before_hide`

Called before show/hide dropdown.

###`combo_init`

Combobox init event.

###`update_position`

Called just before update the position of the dropdown. This even receive offset object, so you can easily change the dropdown position.