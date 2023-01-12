# orcus-getter
a orcus extension for getter attributes for classes

## Dependencies
- [orcus](https://github.com/alphafantomu/orcus)

## Installation
- Make sure you have [luvit](https://luvit.io/install.html) installed
- Run the command `lit install alphafantomu/orcus-getter`
- `require('orcus-getter')` to reference the library

- There is no [LuaRocks](https://luarocks.org/) release, but only `init.lua` is necessary to use the library.

## Usage
The usage is really simple `getter(closure_function, should_cache)`, here is an example

```lua
local getter = require('orcus-getter');
local block = require('orcus', {
	nickname = 'Three Dimensional Square';
});

block.name = getter(function(self)
	return self.nickname;
end, true); -- cache the value

print(block.name); --"Three Dimensional Square"
```

## License
This project has an [MIT license](/LICENSE)

## Contact
- Discord: `Arivistraliavatoriar#2678`