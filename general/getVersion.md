<!-- This file was generated by the script. Do not edit it, any changes will be lost! -->

## getVersion()



Returns OpenTX version

### Example

This example also runs in OpenTX versions where the radio version was not available:

```lua
local function run(event)
  local ver, radio = getVersion()
  print("version: "..ver)
  if radio then print ("radio: "..radio) end
  return 1
end

return {  run=run }
```
Output of above script in simulator:
```
version: 2.1.7
radio: taranis-simu
Script finished with status 1
```


#### Parameters

none

#### Return value

* `string` OpenTX version (ie "2.1.5")

* `list` (available since OpenTX 2.1.7) returns two values:
 * `string` OpenTX version (ie "2.1.5")
 * `string` radio version: `taranisx9e`, `taranisplus` or `taranis`. 
If running in simulator the "-simu" is added



