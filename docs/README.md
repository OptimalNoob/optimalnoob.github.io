> ## string_wordwrap
>
> This function will return a string that has line-break characters inserted into it. Line-breaks are added based on the `max_width` value provided in the function, the max_width is the width (in pixels) on screen that the current "line" has to reach before a line-break is added. This function can also optionally split words instead of wrapping before a long word using the `split_word` argument.

<br>

**Syntax:**

```gml
string_wordwrap(str, max_width, break_char, split_word);
```

<br>

| Argument   | Type       | Description                                         |
| :--------- | :--------- | :-------------------------------------------------- |
| str        | **String** | String of text to apply word-wrapping to.           |
| max_width  | **Real**   | Maximum pixel width before a line-break.            |
| break_char | **String** | Line break character to insert into text.           |
| split_word | **Bool**   | Whether or not to split words in half when wrapping |

<br>

**Returns:**

> **String**

<br>

**Example:**

```gml
var dialog = "This is a very long string that would require word-wrapping to avoid the text from trailing off the screen in the game";
var new_dialog = string_wordwrap(dialog);
draw_text(x, y, new_dialog);
```

This will take the original string of test and apply the word-wrap function to it, before storing it into another local variable to be used instead.
