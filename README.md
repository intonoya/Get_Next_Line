# Get_Next_Line

Get_Next_Line is a function, that reads from a file descriptor and returns one line at a time until the end of the file or an error occurs.

## Functionality

- **Repeated Calls**: Multiple calls to the `get_next_line` function (e.g., in a loop) allow you to read the file line by line.
- **Return Values**:
  - If a line is read successfully, the function returns that line including the newline character `\n`.
  - If there's nothing else to read or if an error occurs, the function returns `NULL`.
- **Error Handling**: The function handles cases where the file changes between calls to `get_next_line` or when reading a binary file.
- **Buffer Size**: The buffer size is defined using the `-D BUFFER_SIZE=n` compiler option. This size determines the amount of data read from the file descriptor at once.
