# GDSercomm
GDNative Serial port communication

**Dependencies:**

- `libsercomm`: https://github.com/ingeniamc/sercomm
- `godot-headers`: https://github.com/GodotNativeTools/godot_headers

**Contents:**

Available functions:

- `open(port,baudrate,timeout,bytesz,parity, stop_byte)`

- `(string) read()`

- `(int) read(true)`	(Read raw value)

- `write(string)`

- `get_available()`

- `flush(queue)`

- `list_ports()`

- `close()`

You can get extra info of a function using `get_documentation(function_name)` if you have a godot editor with *nativescript1.1* support.

**Building with scons:**

You first need to add the dependencies to the main folder.
By default it will require a folder named "godot_headers" and a folder named "sercomm"
Add a compiled sercomm shared library (.dll , .so, .dylib) to the "lib" folder
Use the following command:

```sh
scons p=platform
```

Note: At the moment on linux you need to copy the libsercomm.so to /usr/lib/ and run `ldconfig`
