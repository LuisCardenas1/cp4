# cp4 Luis Cardenas

2/14
ChatGPT
Is like a calculator
Can be used for test/labs
Can give similar responses to simliar instances
Can be used to desribe images
Can write code but must know what you are asking for it to do
Has flaws

2/16
Immutable Classes and Inheritance
  Is it possible to make a class so that it cannot be extended
    public final class ClassName
  This must be done with all immutable classes
  If unsure, make class final
    Can always remove later
    Once you let people extend a class, you can't make changes

Exceptions
Chalenges to Building Robust Software
  Software will often be used in conditions that you cannot precisely anticipate
  A user might enter data that is correct
  A user programmer might create or manipulate objects in incorrect ways
  Programmatic operations might fail
  System errors might occur
Technniques for Highlighting Erros
  When an error occurs, we can use:
    System.out.println()
      Create a log file that keeps track of every important event/operation inside your code(including errors). Log4J is a tool for doing this.
    Return a value that indicates an error
    System.exit(): halt execution of your program
Exceptions
  NullPointerException
  IndexOutOfBoundsException
  IOException
 These cause your program to halt
  Show the file and line number where the failure occured 
  Show the "stack trace" - the nested list of method class that brought us to the failure
Examples
  Method calls on uninstantiated objects
  Creating arrays of negative size
  Accessing elements of an array that don't exist
Syntax
  try
    {
      // some code that could throw an exception
    }
    catch (Exception e)
    {
      // fix the problem here
    }
    finally
    {
      // finish things up
    }
 If you're not going to fix the problem there is no reason to catch the Exception
Throwing Exceptions
  When an exception is thrown:
    Execution stops immediately
    JVM examines the call stack for a matching catch statement
    Execution continues within the body of the matching catch statement
    Then: execution continues after the try-catch
 
