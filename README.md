# LuaScriptInstance

Library to expose access for getting and setting the current script instance.

# Installation
You can use LuaScriptInstance in your own project by adding this project as a [Defold library dependency](http://www.defold.com/manuals/libraries/). Open your game.project file and in the dependencies field under project add:

https://github.com/DanEngelbrecht/LuaScriptInstance/archive/master.zip

Or point to the ZIP file of a [specific release](https://github.com/DanEngelbrecht/LuaScriptInstance/releases).

# Usage
Once the dependecy is added two Lua functions are available:
`lua_script_instance.Get()` and `lua_script_instance.Set(instance)`

# LuaScriptInstance API

### lua_script_instance.Get()
Gets the current script instance. The returned value is an opaque type and you should only use it to set the current instance.

**RETURN**
* ```instance``` (opaque) - the current script instance

### lua_script_instance.Set(instance)
Sets the current script instance. The instance parameters must be a value returned by lua_script_instance.Get().

**PARAMETERS**
* ```instance``` (opaque) - the script instance to set
