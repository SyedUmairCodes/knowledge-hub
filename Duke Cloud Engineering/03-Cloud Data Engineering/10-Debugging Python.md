# Debugging Python code
Using print statements to debug involves strategically placing `print` statements within your code to display the values of variables, the flow of execution, and other relevant information at various points. This technique is straightforward and effective for identifying simple errors and understanding the program's behavior.

The use of f-strings (formatted string literals) to create more informative and readable output by embedding variable values directly into the strings. Include type information using the `type()` function within the `print` statements, helping to pinpoint errors caused by unexpected data types.

The Python Debugger is a powerful interactive source code debugger for Python. It allows you to step through your code line by line, inspect variables, set breakpoints, and evaluate expressions, providing a granular level of control for debugging complex issues.

PDB is useful when you need to investigate a specific section of code in detail, particularly when `print` statements alone are insufficient to pinpoint the problem. You can initiate PDB using `import pdb; pdb.set_trace()` within your code, pausing execution at that point and providing an interactive prompt.

Once in the PDB prompt, you can use commands like `n` (next) to step to the next line, `p` (print) to display variable values, and `c` (continue) to resume execution.

While not strictly a debugging technique itself, writing comprehensive tests for your code is an essential practice for preventing and identifying bugs early in the development process. By creating tests that cover various scenarios and edge cases, you can systematically verify the behavior of your code and catch potential issues before they impact users.

In addition to these three primary methods, exception handling using `try-except` blocks as a way to gracefully handle errors and provide informative feedback to users. 
