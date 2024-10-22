**Shell Scripting Basics Cheat Sheet - @csaba_kissi**

# 1. Define a shebang (specify the interpreter)
```bash
#!/bin/bash
```

# 2. Print a message to the terminal
```bash
echo "Hello, World!"
```

# 3. Define a variable
```bash
my_var="Hello"
```

# 4. Access a variable (use $ symbol)
```bash
echo $my_var
```

# 5. Simple if statement
```bash
if [ condition ]; then
    # Commands if condition is true
    echo "Condition is true"
fi
```

# 6. If-else statement
```bash
if [ condition ]; then
    echo "Condition is true"
else
    echo "Condition is false"
fi
```

# 7. For loop
```bash
for i in {1..5}; do
    echo "Iteration $i"
done
```

# 8. While loop
```bash
count=1
while [ $count -le 5 ]; do
    echo "Count: $count"
    ((count++))
done
```

# 9. Read input from user
```bash
read -p "Enter your name: " name
echo "Hello, $name!"
```

# 10. Define a function
```bash
my_function() {
    echo "This is a function!"
}
```

# 11. Call a function
```bash
my_function
```

# 12. Pass arguments to a script
```bash
# Access arguments with $1, $2, etc.
echo "First argument: $1"
echo "Second argument: $2"
```

# 13. Check for file existence
```bash
if [ -f "filename.txt" ]; then
    echo "File exists"
else
    echo "File does not exist"
fi
```

# 14. Logical AND
```bash
if [ condition1 ] && [ condition2 ]; then
    echo "Both conditions are true"
fi
```

# 15. Logical OR
```bash
if [ condition1 ] || [ condition2 ]; then
    echo "At least one condition is true"
fi
```

# 16. Case statement (switch-like structure)
```bash
case "$variable" in
    "value1") echo "Value is 1";;
    "value2") echo "Value is 2";;
    *) echo "Default case";;
esac
```

# 17. Exit a script with a status code
```bash
exit 0
```

# 18. Redirect output to a file
```bash
echo "Output to file" > output.txt
```

# 19. Append output to a file
```bash
echo "Append to file" >> output.txt
```

# 20. Chain commands (execute command1, then command2)
```bash
command1 && command2 # Executes command2 only if command1 succeeds
command1 || command2 # Executes command2 only if command1 fails
``` 