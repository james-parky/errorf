# errof

errorf is a C library for creating gcc style error and warning messages.

## Usage

To generate gcc style error messages you can simply call `print_error_header()` with a valid file name, line and column number, reason, and supplmentary message:
```C
#include "errorf.h"
print_error_header("file.c", 10, 11, "invalid syntax",
                   "a variable name cannot contain an underscore");
```
This would generate the following error message in the terminal:
```console
file.c:10:11: error: invalid syntax: a variable name cannot contain an underscore
this is an example of a line containing a syntax error in column 11;
           ^~~~~~~    
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.
