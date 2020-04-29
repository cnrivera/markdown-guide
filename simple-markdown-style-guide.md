# A Simple Markdown Style Guide (Written in Basic Markdown)

by Noel Rivera\
28 April 2020

***

## A Brief Introduction

This guide to markdown is intended to serve as an example of what it is explaining.
Examine the markdown file while using the markdown previewer in your text editor of choice to see how the text looks when rendered.

### **What version of markdown are we using?**

I based this guide on the **CommonMark** style.
To read up on it, get links to other markdown extensions, and run through a brief interactive markdown tutorial, visit <https://commonmark.org/>.

### Additional Notes

* *Single return* refers to hitting `Enter` once.
* *Double return* refers to hitting `Enter` twice.
* The backslash `\` character can be used as an escape character to stop formatting on characters with special meanings, such as the asterisk (`*`), period (`.`), dash (`-`), or backslash itself. This is pointed out occasionally in the document.
* This file's appearance will render differently depending on which text editor or viewer you use. 
* If you would like to view rendered markdown in your Chrome web browser, install the Markdown Viewer Chrome extension.
* Feedback, suggestions, or questions about this document can be sent to cnrivera@gmail.com.

***
***
## Horizontal Rules

To create a **horizontal rule**, use a double return, then type `***` or `---` on its own line.

***

## Header Styles

Similar to HTML headers, markdown headers range in size from 1 - 6 depending on the number of hashtags `#` used before the header text.

# Header 1: `#` followed by a space

## Header 2: `##` followed by a space

### Header 3: `###` followed by a space

#### Header 4: `####` followed by a space

##### Header 5: `#####` followed by a space

###### Header 6: `######` followed by a space

***

## Paragraph Styling

To **continue writing in the same paragraph**, use a single return after each sentence. Yes, you *could* just keep writing, but limiting it to one sentence per line makes the markdown file more readable.

To create **a new paragraph** (aka a hard return), use a double return and begin your next paragraph after the blank line.

To create **a soft return**\
use a backslash `\`\
after each line\
to make your words drop\
to the next line\
without creating\
a new paragraph,\
like in a poem,\
or an HTML \<br>.

You can also  
accomplish the same thing  
using two spaces  
after each line,  
but it's harder  
to know  
exactly  
what's going on   
in the file.

***

## Emphasis Styling

To create *italic text*, wrap it in single asterisks `* *` or single underscores `_ _`.

To create **bold text**, wrap it in double asterisks `** **` or double underscores `__ __`.

If you want to **use asterisks or underscores as part of your text** rather than to format emphasis, add a backslash in front of the symbols: `\*` or `\_`.

***

## Nested Paragraphs and Block Quotations

To create **nested paragraphs**:

    Start the nested portion with a double return followed by four spaces at the beginning of your sentence.

    Create a new paragraph in a nested paragraph the same way you would a regular paragraph.
    Just make sure you still have the four spaces before the sentence.

    Nested paragraphs are essentially a different way of making a code block (more on this later).

To create **block quotations**:
> Start your sentence with a caret `>` followed by an optional space.
>
> When making **new paragraphs in a block quotation**, use a double return, as usual, but *make sure there is a caret* `>` *on the blank line*.

> Otherwise you'll end up with two blocks intead of one.
> > You can create nested block quotations by using two carets `> >` before the line.

***

## List Styling

1. To create an **ordered list**, type your number followed by a period `.` and a space.
2. Ordered list with nested sub-list
   1. To create a **nested ordered sub-list**, add four spaces to the beginning of your next list item.

* To create an **unordered list**, type an asterisk `*`, dash `-`, or plus `+` followed by a space.
    * The symbol you use is a matter of preference.
* To create a **nested unordered sub-list**:
    * Add four spaces to the beginning of your next list item.
         * A **second nested sub-list** adds another four spaces to the beginning of the item (for a total of eight).

1. To **add a soft return or paragraph to a list item**:\
    *Soft return*: Use the backslash `\` at the end of the first paragraph, a single return, and four spaces at the start of the next line. 

    *Paragraph*: Or use a double return and four spaces before the line to create a separated paragraph beneath the original list item.

3\. Want to **place a number at the beginning of your paragraph** without turning it into an ordered list? Use the backslash `\` before the period.

***

## Code Styling
To **format inline code**, wrap your code in single tick marks \` \` . Your code will look like this: `x = 25`, therefore `x / 5 = 5`.

To create **a code block**, wrap your code in a code fence by typing three tick marks \`\`\` on the line before your code and on the line after.
*Note:* If you do not close the block, the rest of the page will become part of the block.

```
namespace CSharpTutorials
{
    class Program
    {
        static void Main(string[] args)
        {
            string message = "Hello World!!";

            Console.WriteLine(message);
        }
    }
}
```

You can also create **nested code blocks** the same way you create nested paragraphs and nested lists: add four spaces before your lines.
```
int x = 5;
int y = 10;

    Console.WriteLine("When would you need this?")
    Console.WriteLine("I'm sure there's an example.")
    Console.WriteLine("Don't forget to close your code block.")

```
***

## Link Styling

**Inline linking** uses carets `< >` to wrap the link and make it clickable.
For instance: `<http://www.codecademy.com>` becomes <http://www.codecademy.com>.
However, you must include the `http://` or `https://`, or it won't work properly.

If you want to **assign text to a link**, use `[ ]` to wrap the text, followed by `( )` to wrap the URL. For instance, `[learn to code for free](http://www.freecodecamp.org)` becomes [learn to code for free](http://www.freecodecamp.org).

**Reference linking** allows you to **assign the same link to multiple instances of text**. To do so, surround the text you want linked with square brackets `[The text]` followed by the number of the link in another set of brackets `[1]` (you can have multiple links, therefore multiple numbers). Beneath your finished paragraph, list your number in square brackets followed by a colon`[1]:`, then add your link URL.

For example, this . . .

```
[JavaScript][1], often abbreviated as JS, is a programming language that conforms to the ECMAScript specification. [JavaScript][1] is high-level, often just-in-time compiled, and multi-paradigm.

[1]:https://en.wikipedia.org/wiki/JavaScript
```

. . . becomes this:

[JavaScript][1], often abbreviated as JS, is a programming language that conforms to the ECMAScript specification. [JavaScript][1] is high-level, often just-in-time compiled, and multi-paradigm.

[1]:https://en.wikipedia.org/wiki/JavaScript

***

## Adding Images

To **add an image**, use an exclamation mark followed by square brackets, followed by the image URL in parentheses: `![optional-alt-tag](http://somelink.com)`. You can add an alt tag between the square brackets, if desired.

The image will render as shown below:

![optional-alt-tag](https://commonmark.org/help/images/favicon.png)

***
***
### Thank you for reading! 