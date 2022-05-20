# Z Header Files Explained

Here's what [[z header]] looks like:

```markdown
<% $foo = "---" %>
author: Gustavo DeLaFuerza
date created: <% tp.date.now("YYYY-MM-DDTHH:mm:ssZ\Z") %>
date modified: <% tp.date.now("YYYY-MM-DDTHH:mm:ssZ\Z") %>
<% $foo = "---" %>
```

## Line by line

Here's what's going on:

`<% $foo = "---" %>` is my way of rendering three dashes at the top of the file to begin YAML metadata.  I use the same thing for the bottom of the YAML tag. 

Rendering the three dashes keeps Obsidian from treating this header file as having header content in it. This makes it display more nicely in Obsidian based on my personal preference.

One doesn't need to have metadata at the top of their files. It might hamper more than help. 

For me, I like having the metadata.

The next line is "author", then `date created: <% tp.date.now("YYYY-MM-DDTHH:mm:ssZ\Z") %>`, which Templater code I also use for "date modified". It displays a standard time (UTC) in the format for today's date of 2022-05-16T10:03:00-04:00Z. The "-04:00" is represented by 'Z', the 'T' is rendered only as the letter itself, and because 'Z' represents the difference of time from GMT (Greenwich Mean Time), it has to be escaped with a double-backslash to display the letter 'Z'. Fun stuff. 

In my personal vault, I have the Linter plugin set to put the same metadata at the top of a page (e.g. one I create ad-hoc, not by-template).