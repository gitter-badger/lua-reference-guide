<!-- This file was generated by the script. Do not edit it, any changes will be lost! -->

## model.setGlobalVariable(index, phase, value)



Sets current global variable value. See also model.getGlobalVariable()


#### Parameters

* `index`  zero based global variable index, use 0 for GV1, 8 for GV9

* `phase`  zero based phase index, use 0 for Phase 1, 5 for Phase 6
   
* `value`  new value for global variable. Permitted range is
from -1024 to 1024. 
    



#### Return value

none

##### Notice
Global variable can only store integer values, 
any floating point value is converted (todo check how) into integer value.




---

### Examples

### Example

this is a sample example


![](setGlobalVariable-example05.png)

```lua
function foo(bar)
  local x = bar * 2
end
```

