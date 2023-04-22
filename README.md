<div style="background-color:#05BFDB"><font size="18" color="black" type="Helvetica">Basic Syntax </font> 
<h4> The Markdown elements outlined in the original design document.</h4></div>

***

## Overview

Nearly all Markdown applications support the basic syntax outlined in the original Markdown design document. There are minor variations and discrepancies between Markdown processors — those are noted inline wherever possible.

## Headings

To create a heading, add number signs (#) in front of a word or phrase. The number of number signs you use should correspond to the heading level. For example, to create a heading level three (\<h3>), use three number signs (e.g., ### My Header).

| Markdown | HTML | Rendered Output |
|----------|------|-----------------|
|\# Heading level 1| \<h1>Heading level 1</h1>| <h1>Heading level 1</h1>|
|\## Heading level 2|\<h2>Heading level 2</h2>| <h2>Heading level 2</h2>|
|etc.|etc.|<h3>etc.</h3>|

## Alternate Syntax

Alternatively, on the line below the text, add any number of == characters for heading level 1 or -- characters for heading level 2.

| Markdown | HTML | Rendered Output |
|----------|------|-----------------|
|Heading level 1 <br>============|\<h1>Heading level 1</h1>|<h1>Heading level 1</h1>|
|Heading level 2 <br>---------------------|\<h2>Heading level 2</h2>|<h2>Heading level 2</h2>|

## Heading Best Practices

Markdown applications don’t agree on how to handle a missing space between the number signs (#) and the heading name. For compatibility, always put a space between the number signs and the heading name.

|✅ Do This| ❌ Don't Do This|
|-----------|-----------------|
|\# Here's a Heading|#Here's a Heading|

You should also put blank lines before and after a heading for compatibility.

|✅ Do This| ❌ Don't Do This|
|-----------|-----------------|
|Try to put a blank line before... <br><br>\# Heading <br><br>...and after a heading.|Without blank lines, this might not look right.<br>\# Heading<br>Don't do this!|

## Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text.

| Markdown | HTML | Rendered Output |
|----------|------|-----------------|
|I really like using Markdown.<br><br>I think I'll use it to format all of my documents from now on.|\<p>I really like using Markdown.</p><br>\<p>I think I'll use it to format all of my documents from now on<br>\</p>|<p>I really like using Markdown.</p><br><p>I think I'll use it to format all of my documents from now on.</p>|

## Paragraph Best Practices

Unless the paragraph is in a list, don’t indent paragraphs with spaces or tabs.
