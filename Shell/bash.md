# Bash Cheatsheet

## Variables

To declare a variable in Bash, use the following syntax:

```bash
variable_name=value
```

To access the value of a variable, use the `$` symbol followed by the variable name:

```bash
echo $variable_name
```

## Conditionals

To perform conditional checks in Bash, use the `if` statement:

```bash
if [ condition ]; then
    # code to be executed if condition is true
else
    # code to be executed if condition is false
fi
```

## Loops

Bash provides several types of loops, including `for`, `while`, and `until` loops. Here's an example of a `for` loop:

```bash
for item in list; do
    # code to be executed for each item in the list
done
```

## Functions

To define a function in Bash, use the following syntax:

```bash
function_name() {
    # code to be executed
}
```

To call a function, simply use its name followed by parentheses:

```bash
function_name
```

## File Operations

Bash provides various commands for file operations, such as `touch`, `rm`, `mv`, and `cp`. Here's an example of using the `touch` command to create a new file:

```bash
touch filename
```

## Command Line Arguments

To access command line arguments in Bash, you can use the special variables `$1`, `$2`, `$3`, and so on, where `$1` represents the first argument, `$2` represents the second argument, and so on.

## Conclusion

This cheatsheet provides a brief overview of some commonly used features in Bash. For more detailed information, refer to the Bash documentation.
