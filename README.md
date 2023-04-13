# practical-haxe

After a year of working with haxe, here's a few things i wish i'd known at the start. this page looks at haxe from a realtime perspective, with a bias towards games

# Targets
* hashlink - rapid iteration, excellent support, reasonable performance
* hxcpp - slower iteration, reasonable support, excellent performance
* jvm - fast iteration, developing support, strong performance (some memory bloat)
* js - tbd

# Workflow
+ vscode + code completion
  + A really solid combination, and my recommended workflow
  + You often have to restart the code completion with large projects (Use the command pallete)
+ compilation server
  + you can find the instructions here: https://haxe.org/manual/cr-completion-server.html
+ haxelib vs git
  + Haxelib has lots of libraries, however, many of them are out of date
  + Haxelib is natively integrated into the Haxe compiler, which makes it the default package manager
  + Many modern Haxe libs are only distributed through git, and often require you to keep dependencies up to date


# Recommended Libraries
There are lots of long lists of libs, but i'm going to try to recommend only one, at most two for a given category.

## Macros
* tink macro - when used properly, makes macros easier to write.

## async
* pecan

## native extension shims
* ammer - Supports good subset of targets, the defacto default
* h-idl [RC] - An alternative primarily supporting Hashlink with a lot of features for additional perf

## logging
* hlog [RC] - A very lightweight trace-like logging suite

## game engine
### Heaps
Runs on Hashlink
* heaps.io
* hide - extends heaps with an editor
  * Requires you to keep heaps and hashlink up to date through git

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





