# GDSercomm
GDNative Serial port communication

**Dependencies:**

- libsercomm: https://github.com/ingeniamc/sercomm
- godot-headers: https://github.com/GodotNativeTools/godot_headers

**Contents:**

Available functions:

- open(*port,baudrate,timeout,bytesz,parity, stop_byte*)

- (**string**) read()

- write(*string*)

- get_available()

- flush(queue)

- list_ports()

- close()

You can get extra info using *get_documentation(function_name)* if you have a godot editor with *nativescript1.1* support.
