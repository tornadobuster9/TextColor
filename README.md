# TextColor
A Java library that lets your print formatted text using ANSI color codes. It's simple and lightweight, and very easy to use!

## How to use
Using the API is very simple. Start by importing the com.libs.textcolor.main.TextColor class.
For example:

```java
import com.libs.textcolor.main.TextColor;

public class TextColorTest {
  public static final void main(String[] args) {
    System.out.println(TextColor.ANSI_FG_RED + "This text will be in red." + TextColor.ANSI_ALL_RESET);
  }
}
```
would print "This text will be in red." to the console, in red.

## Notes
IMPORTANT: Not all ANSI color codes are supported by every terminal! Most codes here are not supported by the Windows Command Prompt. If you're looking for an ANSI library that supports Windows, I recommend checking out the [Jansi](https://github.com/fusesource/jansi) library.

If you're using an IDE, chances are that the codes will not display into the built-in console. You will need to export it first, then you can run it from the command prompt.
