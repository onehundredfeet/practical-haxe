# practical-haxe

After a year of working with haxe, here's a few things i wish i'd known at the start. this page looks at haxe from a realtime perspective, with a bias towards games

# Targets
* hashlink - rapid iteration, excellent support, reasonable performance
* hxcpp - slower iteration, reasonable support, excellent performance
* jvm - fast iteration, developing support, strong performance (some memory bloat)
* js - tbd

## Target Benchmarks
https://benchs.haxe.org


# Workflow
+ VS Code + Code Completion
  + Install the Haxe extension from the marketplace  
  + A really solid combination, and my recommended workflow
  + You often have to restart the code completion with large projects (Use the command pallete)
+ Compilation server
  + Use this to massively speed up iterative compilations
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
* h-idl [RC] - An alternative primarily supporting Hashlink with a lot of features for additional perf, some assembly required

## logging
* hlog [RC] - A very lightweight trace-like logging suite

## Game Engine
### Heaps
Runs on Hashlink
* heaps.io
* hide - extends heaps with an editor
  * Requires you to keep heaps and hashlink up to date through git

## Game Serialization / Networking
* hxbit - macro based serialization

## ECS
* hmecs [RC] - Plug for my own fork of echoes, a macro based ECS

## Bit Packing
* hbitsignals [rc] provides a simple franework for writing very dense bit streams

## Unit Testing
* buddy

## Media Reading and writing 
* format

## Threading
* sys.threads - Built in for any sys supporting target.  Faster than haxe-concurrent









