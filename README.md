# information
a) to use this in studio, you could create a `ModuleScript` and put the `src.lua` contents or just make it a function within your own script

b) if you want to use this for exploit environment development, just simply make an http request to the raw `src.lua` contents file or make a function within the script and call it from there

```lua
notify( <string> text, <Color3> color, <number> expiration )
```

# exploit environment usage
```lua
local notify = loadstring( game:HttpGetAsync( 'https://raw.githubusercontent.com/networktraffic/blaze/main/src.lua' ) )( )
notify( 'hello world', Color3.new( 1, 1, 1 ), 3 )
```
