# errof

errorf is a C library for creating gcc style error and warning messages.

## Usage

```C
#include "errorf.h"
print_error_header(file, 10, 15, "invalid syntax",
                   "a variable name cannot contain an underscore");
/*
file:10:15: error: invalid syntax: a variable name cannot contain an underscore
*/

#include "errorf.h"
print_warning_header(file, 10, 15, "invalid syntax",
                     "a variable name cannot contain an underscore");
/*
file:10:15: warning: invalid syntax: a variable name cannot contain an underscore
*/
```


## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.
