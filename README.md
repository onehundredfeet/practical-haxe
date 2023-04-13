# practical-haxe

After a year of working with haxe, here's a few things i wish i'd known at the start. this page looks at haxe from a realtime perspective, with a bias towards games

# Targets
* hashlink - rapid iteration, excellent support, reasonable performance
  * Profiling - [Instructions](https://github.com/HaxeFoundation/hashlink/wiki/Profiler)
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
+ haxe vs 

# Recommended Libraries
There are lots of long lists of libs, but i'm going to try to recommend only one, at most two for a given category.

## Macros
* tink macro - when used properly, makes macros easier to write.

## Async
* pecan

## Native Extension Shims
* ammer - Supports good subset of targets, the defacto default
* h-idl [RC] - An alternative primarily supporting Hashlink with a lot of features for additional perf, some assembly required

## Logging
* hlog [RC] - A very lightweight trace-like logging suite

## Game Engine
### Heaps
Runs on Hashlink & JS
* heaps.io [Github](https://github.com/HeapsIO/heaps) 
* hide - extends heaps with an editor [Github](https://github.com/HeapsIO/hide)
  * Requires you to keep heaps and hashlink up to date through git

### Flixel [Github](https://github.com/HaxeFlixel/flixel)
* I do NOT use this, but lots of people do, so investigate on your own

## Game Serialization / Networking
* hxbit - macro based serialization [Github](https://github.com/HeapsIO/hxbit)

## Game Database
* CastleDB

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

## 3D Math
* hvector

## Random numbers
* seedyrng

## Tool / App UI
* Haxe-ui [Github](https://github.com/haxeui)
  * Top notch, excellent for tools and apps

## Game UI
  * Heaps + Domkit [Github](https://github.com/HeapsIO/domkit)

# Community
The Haxe discord is the most active place I've been able to find.







