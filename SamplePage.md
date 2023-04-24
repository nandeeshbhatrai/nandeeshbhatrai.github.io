<div style="background-color:#FFFBF5 ; padding:5px"><div style="background-color:#00D7FF ; padding:10px"><font size="18" color="black" type="Helvetica">Basic Syntax </font> 
<h4> The Markdown elements outlined in the original design document.</h4></div>

---

## <div id="overview">Overview</div>

Nearly all Markdown applications support the basic syntax outlined in the original Markdown design document. There are minor variations and discrepancies between Markdown processors — those are noted inline wherever possible.

## Headings

To create a heading, add number signs (#) in front of a word or phrase. The number of number signs you use should correspond to the heading level. For example, to create a heading level three (\<h3>), use three number signs (e.g., ### My Header).

| Markdown            | HTML                      | Rendered Output          |
| ------------------- | ------------------------- | ------------------------ |
| \# Heading level 1  | \<h1>Heading level 1</h1> | <h1>Heading level 1</h1> |
| \## Heading level 2 | \<h2>Heading level 2</h2> | <h2>Heading level 2</h2> |
| etc.                | etc.                      | <h3>etc.</h3>            |

## Alternate Syntax

Alternatively, on the line below the text, add any number of == characters for heading level 1 or -- characters for heading level 2.

| Markdown                                  | HTML                      | Rendered Output          |
| ----------------------------------------- | ------------------------- | ------------------------ |
| Heading level 1 <br>============          | \<h1>Heading level 1</h1> | <h1>Heading level 1</h1> |
| Heading level 2 <br>--------------------- | \<h2>Heading level 2</h2> | <h2>Heading level 2</h2> |

## Heading Best Practices

Markdown applications don’t agree on how to handle a missing space between the number signs (#) and the heading name. For compatibility, always put a space between the number signs and the heading name.

| ✅ Do This          | ❌ Don't Do This  |
| ------------------- | ----------------- |
| \# Here's a Heading | #Here's a Heading |

You should also put blank lines before and after a heading for compatibility.

| ✅ Do This                                                                           | ❌ Don't Do This                                                                |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------- |
| Try to put a blank line before... <br><br>\# Heading <br><br>...and after a heading. | Without blank lines, this might not look right.<br>\# Heading<br>Don't do this! |

## Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text.

| Markdown                                                                                            | HTML                                                                                                                | Rendered Output                                                                                               |
| --------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| I really like using Markdown.<br><br>I think I'll use it to format all of my documents from now on. | \<p>I really like using Markdown.</p><br>\<p>I think I'll use it to format all of my documents from now on<br>\</p> | <p>I really like using Markdown.</p><br><p>I think I'll use it to format all of my documents from now on.</p> |

## Paragraph Best Practices

Unless the <a href="https://www.markdownguide.org/basic-syntax/#paragraphs">paragraph is in a list</a>, don’t indent paragraphs with spaces or tabs.

| Markdown                                                                                            | HTML                                                                                                            | Rendered Output                                                                                               |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| I really like using Markdown.<br><br>I think I'll use it to format all of my documents from now on. | \<p>I really like using Markdown.</p><br>\<p>I think I'll use it to format all of my documents from now on.</p> | <p>I really like using Markdown.</p><br><p>I think I'll use it to format all of my documents from now on.</p> |

## Line Breaks

To create a line break or new line (<br>), end a line with two or more spaces, and then type return.

| Markdown                                                 | HTML                                                                  | Rendered Output                                                |
| -------------------------------------------------------- | --------------------------------------------------------------------- | -------------------------------------------------------------- |
| This is the first line. <br>And this is the second line. | \<p>This is the first line.\<br> <br>And this is the second line.</p> | <p>This is the first line.<br>And this is the second line.</p> |

## Line Break Best Practices

You can use two or more spaces (commonly referred to as “trailing whitespace”) for line breaks in nearly every Markdown application, but it’s controversial. It’s hard to see trailing whitespace in an editor, and many people accidentally or intentionally put two spaces after every sentence. For this reason, you may want to use something other than trailing whitespace for line breaks. If your Markdown application <a href="https://www.markdownguide.org/basic-syntax/#html">supports HTML</a>, you can use the \<br> HTML tag.

For compatibility, use trailing white space or the \<br> HTML tag at the end of the line.

There are two other options I don’t recommend using. CommonMark and a few other lightweight markup languages let you type a backslash (\\) at the end of the line, but not all Markdown applications support this, so it isn’t a great option from a compatibility perspective. And at least a couple lightweight markup languages don’t require anything at the end of the line — just type return and they’ll create a line break.

| ✅ Do This                                                                                                                     | ❌ Don't Do This                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
| First line with two spaces after. <br>And the next line.<br><br>First line with the HTML tag after.\<br><br>And the next line. | First line with a backslash after.\<br>And the next line.<br><br>First line with nothing after.<br>And the next line. |

## Emphasis

You can add emphasis by making text bold or italic.

## Bold

To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.

| Markdown                       | HTML                                      | Rendered Output                         |
| ------------------------------ | ----------------------------------------- | --------------------------------------- |
| I just love \*\*bold text\*\*. | I just love \<strong>bold text\</strong>. | I just love <strong>bold text</strong>. |
| I just love \_\_bold text\_\_. | I just love \<strong>bold text\</strong>. | I just love **bold text**.              |
| Love\*\*is\*\*bold             | Love\<strong>is\</strong>bold             | Love**is**bold                          |

## Bold Best Practices

| ✅ Do This         | ❌ Don't Do This |
| ------------------ | ---------------- |
| Love\*\*is\*\*bold | Love**is**bold   |

## <div id="italics">Italic</div>

To italicize text, add one asterisk or underscore before and after a word or phrase. To italicize the middle of a word for emphasis, add one asterisk without spaces around the letters.

<div style="background-color:#A9E6E6 ; border-radius:5px; padding:7px"><strong>ⓘ NOTE:</strong> The order of the <code>em</code> and <code>strong</code> tags might be reversed depending on the Markdown processor you're using.</div>

<br>

<div :hover="background-color:yellow"><a href="#italics">Go to Italics!</a><br>
<a href="#overview">Go to OverView!</a></div>


