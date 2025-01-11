# Tcl expr command misuse
This repository contains a simple example demonstrating a common error when using the Tcl expr command. The expr command is designed to evaluate mathematical and logical expressions. Using it with strings other than numbers can lead to unexpected results or errors.

## Bug Description
The issue lies in the way the expr command is used within the 'foo' procedure.  The code attempts to add 1 to the string "1", which is an incorrect usage of expr.  This results in a unexpected behavior rather than the integer addition.

## Solution
The solution involves ensuring that the input to expr is correctly handled as a number before being used in the arithmetic expression. This example provides the corrected version of the Tcl code.