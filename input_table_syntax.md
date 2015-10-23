# Input Table Syntax

#####Overview

The input table defines what values are available as input(s) to [mix scripts](mix.md). There are two forms of input table entries.

* #####SOURCE syntax
```lua
{ "<name>", SOURCE }
```
SOURCE inputs provide the current value of a selected OpenTX variable. The source must set by the user when the mix script is configured. Source can be any value OpenTX knows about (inputs, channels, telemetry values, switches, custom functions,...).<br/>
*Note:* see [getValue()](getvalue_function.md) function for proper interpretation of input values.


* #####VALUE syntax
```lua
{ "<name>", VALUE, <min>, <max>, <default> }
```
VALUE inputs provide a constant value that is set by the user when the mix script is configured.

#####Example using a SOURCE and a VALUE
```lua
local input =
    {
        { "Strength", SOURCE},			    -- user selects source (typically slider or knob)
        { "Interval", VALUE, 0, 100, 0 }    -- interval value, default = 0.
    }
    
local function run(strength, interval)
    -- variable strength will contain the current slider value
    -- variable interval is set by the user and constant through script lifetime

    -- ****script has no return value but may use playFile() to alert user

    return
end

return {input=input, run=run}
```
