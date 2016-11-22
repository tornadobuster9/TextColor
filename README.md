# TextColor
A Java library that lets your print formatted text using ANSI color codes. It's simple and lightweight, and very easy to use!

## Installing
To actually use the library, you will need to add it to the Java Build Path. Here are instructions on how to do that in Eclipse:

1. Right-click the project and select "Properties"
2. Select "Java Build Path"
3. Select "Add External Jars..."
4. Navigate to the directory to where you downloaded the TextColor.jar file, and select "Open"

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
You can also combine multiple styles:
```java
import com.libs.textcolor.main.TextColor;

public class TextColorTest {
  public static final void main(String[] args) {
    System.out.println(TextColor.ANSI_BOLD_ON + TextColor.ANSI_FG_RED + "This text will be in red and bold." + TextColor.ANSI_ALL_RESET);
  }
}
```

## Notes
IMPORTANT: Not all ANSI color codes are supported by every terminal! Most codes here are not supported by the Windows Command Prompt. If you're looking for an ANSI library that supports Windows, I recommend checking out the [Jansi](https://github.com/fusesource/jansi) library.

If you're using an IDE, chances are that the codes will not display into the built-in console. You will need to export it first, then you can run it from the command prompt.
