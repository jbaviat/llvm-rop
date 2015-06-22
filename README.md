
# LLVM ROP Gadget generator POC

Tiny llvm-objdump patch which list gadgets found in a binary.

If you are looking for:
 - a gadget generator: please find something else.
 - an LLVM's hack example: please keep reading.

## Compilation

Prepare your LLVM environment for compilation, then:

```shell
$ cd llvm/tools
$ git clone <this repo> 
```

Then build LLVM as usual.


## Usage

```shell
$ llvm-rop /path/to/my/binary
```

## Note

For fat MachO binaries, use lipo to thin them to a single architecture MachO file:

```shell
$ lipo -thin x86_64 /Applications/iTunes.app/Contents/MacOS/iTunes -output /tmp/a
```

