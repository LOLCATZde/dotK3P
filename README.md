# dotK3P
Ruleset for .K3P files, a zip-based file format for the Keksis 3 Patcher.

## What are .K3P files?
The .K3P format is a .ZIP-based "pseudoformat".

The goal of dotK3P is to offer a simple way of marking files for deletion in .ZIP files in a compatible, human-readable manner, without using f.e. long lists.
The very simple usage of a ".2bdeleted" file (can be empty) in a .K3P file marks what file(s) should be deleted by the unpacking program.

## How does a .K3P file look like?
The main intend of the .K3P format is to allow easy patching of private Minecraft modpacks - therefore this example displays a patch for a Minecraft modpack. The .K3P format can be used for anything though, really.

modpack-patch1.k3p
> mods
> > NewExampleModIWantToAdd.jar
> > 
> > CoreModExample.jar
> > 
> > IDontLikeYouAnymore.jar.**2bdeleted**
> > 
> > And-you-neither.jar.**2bdeleted**
> > 
> config
> > NewExampleModIWantToAdd.cfg
> > 
> > IDontLikeYouAnymore-common.toml.**2bdeleted**

## What program would actually use this?
Our own program, [Keksis 3 Patcher](https://github.com/LOLCATZde/Keksis3Patcher) does.

## Final words?
There you go, have fun with it.

Copyright 2024 LOLCATZ.DE
