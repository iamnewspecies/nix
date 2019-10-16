# nix
Figuring out nix

## Highligts of nix pills

The derivation function receives a set as first argument. This set requires at least the following three attributes:

name: the name of the derivation. In the nix store the format is hash-name, that's the name.

system: is the name of the system in which the derivation can be built. For example, x86_64-linux.

builder: it is the binary program that builds the derivation.


Some analogies with the C language:

.nix files are like .c files

.drv files are intermediate files like .o files. The .drv describes how to build a derivation, it's the bare minimum information.

out paths are then the product of the build

