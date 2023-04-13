# practical-haxe

After a year of working with haxe, here's a few things i wish i'd known at the start. this page looks at haxe from a realtime perspective, with a bias towards games

# targets
* hashlink - rapid iteration, excellent support, reasonable performance
* hxcpp - slower iteration, reasonable support, excellent performance
* jvm - fast iteration, developing support, strong performance (some memory bloat)
* js - tbd

# workflow
+ vscode + code completion
++ A really solid combination, and my recommended workflow
++ You often have to restart the code completion with large projects (Use the command pallete)
+ compilation server
++ you can find the instructions here: 
+ haxelib vs git


# recommended libraries

there are lots of long lists of libs, but i'm going to try to recommend only one, at most two for a given category.

## Macros
* tink macro - when used properly, makes macros easier to write.

## async

* pecan

## native extension shims
* ammer
* h-idl

## logging
* hlog [rc]

## game engine
### Heaps
runs on hashlink, requires 
* heaps.io
* hide - extends heaps with an editor

## game serialization / networking
* hxbit - macro based serialization

## bit packing
* hbitsignals [rc] provides a simple franework for writing very dense bit streams

## unit testing
* buddy

## media reading and writing 
* format

## threading
* sys.threads
* haxe-concurrent - not recommended for games





