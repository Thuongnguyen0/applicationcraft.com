---
old_url: getting_widget_data_into_an_ob.htm
title: "Getting Widget Data into an Object"
active_menu_item: developers
class_name: developers
full_width: true
---


The Application Craft **client** API (not the SSJ API) provides a number of functions that help you get data out of your AC App and into an object structure that can be passed easily to your SSJ functions.

## Widget Values

The two main functions for getting widget values are

 - [app.dataGetValues()](/developers/documentation/scripting-apis/client-api/widget-data-state-manipulation/datagetvalues) - gets all, some or a page of Widget values into an object structure suitable for passing to SSJ functions with the minimum of fuss.

 - [app.dataSetValues()](/developers/documentation/scripting-apis/client-api/widget-data-state-manipulation/datasetvalues) - takes an object structure of values and populates any widgets with values from the object where the object key name matches the widget name.

If you are working with SSJ DB functions and you want to avoid the need to write any extra code, then giving your widgets the same name as your database fields will mean that the object structure generated by [app.dataGetValues()](/developers/documentation/scripting-apis/client-api/widget-data-state-manipulation/datagetvalues) will can be used by [ssj.dbInsert()](/developers/documentation/scripting-apis/server-side-api/ssj-object/database/insert) and [ssj.dbUpdate()](/developers/documentation/scripting-apis/server-side-api/ssj-object/database/update) .

## Widget States

There are also functions for getting and setting widget states (visible, enabled and read-only properties).

 - [app.dataGetStates()](/developers/documentation/scripting-apis/client-api/widget-data-state-manipulation/datagetstates) - gets all, some or a page of Widget states into an object structure.

 - [app.dataSetStates()](/developers/documentation/scripting-apis/client-api/widget-data-state-manipulation/datasetstates) - takes an object structure representing widget states and applies it to matching widget names.

## Related Videos

[![Videos\_P](/img/docs/videos_p.png)](http://www.youtube.com/v/qY9M8bP9b70?autoplay=1&hd=1&fs=1&showsearch=0&rel=0&) Coding up client/server side javascript calls [7:24]
