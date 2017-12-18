# NNCE Interpreter

This python interpreter implements the natural number calculation engine as described above.
## Using the interpreter
	python nnce.py --help

The interpreter stores the output tape internally, and writes its full contents to STDOUT when execution halts.

## Implementation Details

### I/O mapping

The NNCE interpreter uses the ASCII character set as its I/O mapping.

### WRITD behavior
WRITD writes the value of the next cell to both STDOUT and the output tape. Note that this doesn't convert to ASCII: It writes the literal number or command stored in the next cell.