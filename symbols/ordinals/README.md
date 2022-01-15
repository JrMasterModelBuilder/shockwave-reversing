# Windows Library Export Ordinals

On macOS, library functions are exported by name. On Windows however, most library functions are exported by ordinal and not name. Most of these functions exist in both libraries and/or libOtto, making it possible to determine the original name for most ordinals. The few platform-specific names that could not recovered from other sources were given names based on their functionality, and are listed in `custom-names.txt`.


## Matching Versions

To find the ordinal names for a version of the library, find the version closest matching the file version number stored in the PE resources. Note that for many versions code was deduplicated by the compiler, so if two exports have the same code that same code will be exported until multiple ordinals.


## Mid-Version Argument Changes

With few exceptions, the number of arguments for exports do not change across these version. Those exceptions are listed below.

```
iml 7.0.0.198 -> 7.0.2.85 1134:imMemPurge (0 args -> 1 args)
iml 11.5.1.601 -> 11.5.2.602 1213:imVsprintf (3 args -> 4 args)
dirapi 8.5.1.102 -> 8.5.1.104 899:TElcr_GetVarInfo (6 args -> 7 args)
dirapi 10.0.0.188 -> 10.0.0.210 168:TESetWindowActive (2 args -> 3 args)
dirapi 10.0.1.4 -> 10.1.0.11 231:TEMiawSetDisplayMode (3 args -> 4 args)
```
