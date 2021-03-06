---
title: dayRender
type: callback
since_version: 1.6
---

A hook for modifying a day cell.

<div class='spec' markdown='1'>
function( date, cell ) { }
</div>

This callback lets you modify day cells that are part of the *month*, *basicWeek*, and *basicDay* views.

`date` is the native Date object for the given day.

You cannot return a new element. You must only modify the `cell` (a `<td>` element) that is provided.

This callback is called each time a cell needs to be freshly rendered. However, a cell does not need to be rerendered when switching views. Rendering only occurs when the calendar navigates to a different date/time.
