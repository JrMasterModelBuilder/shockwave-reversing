# Symbols

Most binaries are stripped of their symbol names, however there are exceptions.


## iOS XDK (`libOtto.a`)

Contains many object files compiled for iOS with tons of symbols.

Available in 32-bit and 64-bit versions.


## iOS APP (`Otto.app`)

A compiled iOS app with `libOtto`, but excludes the private and unused symbols in `libOtto`.

Available in 32-bit and 64-bit versions.


## macOS library exports

On macOS the exported functions have their original symbols.


## Some Windows library exports

On Windows there are some functions which are exported by both ordinal and name.


## Windows 6.0.1.117 16-bit

Some functions have names, though capitalized.


## Director 4 (16-bit)

Many functions have names, though very different from modern versions.


## XDK Versions

The different versions of the XDK also contain a limited set of functions in headers and object files.
