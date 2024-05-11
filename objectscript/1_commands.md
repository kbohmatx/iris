Link: https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_commands#GCOS_commands_pc
A command can take arguments. Exmaples include:

1. If a command takes **one or more arguments**, you must include exactly one space between the command keyword and the first argument. For example: SET X=2
2. **postconditional expression**, there must be **no spaces between the command keyword and the postconditional**. For example: write:count<5 "is greater than 5",!
4. **Argumentless Commands**:  Always argumentless. For example, HALT, CONTINUE, TRY, TSTART, and TCOMMIT are argumentless commands.  Several commands are optionally argumentless. For example, BREAK, CATCH, FOR, GOTO, KILL, LOCK, NEW, QUIT, RETURN, TROLLBACK, WRITE, and ZWRITE all have argumentless syntactic forms
Example of an **argumentless commands**:
 **FOR**  {
    WRITE !,"Quit out of 1st endless loop"
    **QUIT**
 }
 5. 

POST Conditional Syntax:
Command:pc
Example:
  set count = 1
  write:count<5 "is greater than 5",!
Output:
  is greater than 5
