<!-- This file was generated by the script. Do not edit it, any changes will be lost! -->

## getValue(name_or_id)



Returns current value of the requested field. 


#### Parameters

* `name_or_id`  identifier (number) or name (string) of the field



#### Return value

* `value` current field value (number). Zero is returned for:
 * non-existing fields
 * for all telemetry fields when the telemetry stream is not received

* `table` GPS position is returned in a table:
 * `lat` latitude, positive is North (number)
 * `lon` longitude, positive is East (number)

* `table` GPS date/time is returned in a table, format is the same 
as is returned from getDateTime()

* `table` Cells are returned in a table 
(except where no cells were detected in which 
case the returned value is 0):
 * table has one item for each detected cell
 * each item name is the cell number (1 to number of cells)
 * each item value is the current cell voltage



##### Notice
Getting a value by its numerical identifier is faster then by its name.


