# errof

errorf is a C library for creating gcc style error and warning messages.

## Usage

```C
#include "errorf.h"
print_error_header(file, 10, 15, "invalid syntax",
                   "a variable name cannot contain an underscore");
/*
file:10:11: error: invalid syntax: a variable name cannot contain an underscore
this is an example of a line containing a syntax error in column 11;
           ^~~~~~~    
*/

#include "errorf.h"
print_warning_header(file, 10, 15, "invalid syntax",
                     "a variable name cannot contain an underscore");
/*
file:10:11: warning: invalid syntax: a variable name cannot contain an underscore
this is an example of a line containing a syntax warning in column 11;
           ^~~~~~~    
*/
```


## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.
