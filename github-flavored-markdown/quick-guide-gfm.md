
<h1 align="center">Quick Guide: GitHub Flavored Markdown</h1>

<br>

> [!NOTE]
> GitHub Flavored Markdown renders on GitHub related websites (repositories, gists, comments, `.md` files, etc.).

<br>

## Creating an `.md` file

<br>

### Manually
Upload or create a new **Markdown file** by adding the `.md` extension at the end of the file's name.

<br>

### Repository's `README.md`
This file is the first thing people read when they visit your repository, as it helps people understand the repository's content.  
The `README.md` file can be created:
* When creating a new repository, check the option <kbd>Add a README file</kbd>.
* By adding or creating a new file in the root of your repository and naming it `README.md`.

<br>

### Profile `README`
If you want to create a profile README that will show when people visit your GitHub profile homepage, follow these steps:
1. Create a Public repository.
2. Its name must match your username.
3. Check the option <kbd>Add a README file</kbd>.


<br>

More about READMEs, in GitHub Docs:  
- [About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)  
+ [Managing your profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)

---
<br>
 
## Inline Styling
<br>

|  Style           |  Markdown syntax           |  HTML tags                     |  Output Example                 |  Notes                                                           |
|------------------|:--------------------------:|:------------------------------:|:-------------------------------:|------------------------------------------------------------------|
|  Bold            |  `**text**` or `__text__`  |  `<strong>` or `<b>`           |  **text in bold**               |  Keyboard shorcut: <kbd>Command / Ctrl</kbd> + <kbd>B</kbd>      |
|  Italic          |   `*text*`  or  `_text_`   |  `<i>` or `<em>`               |  *text in italic*               |  Keyboard shorcut: <kbd>Command / Ctrl</kbd> + <kbd>I</kbd>      |
|  Strikethrough   |  `~~text~~`                |  `<s>` or `<del>`              |  ~~text with strikethrough~~    |  Single tilde syntax not supported                               | <!-- <strike> tag is depracated, not supported in HTML5 -->
|  Underline       |  -                         |  `<ins> </ins>`                |  <ins>underlined text</ins>     |  -                                                               |
|  Superscript     |  -                         |  `<sup> </sup>`                |  <sup>superscript</sup> text    |  -                                                               |
|  Subscript       |  -                         |  `<sub> </sub>`                |  <sub>subscript</sub> text      |  -                                                               |
|  Highlighting    |  -                         |  `<mark> </mark>`              |  <mark>highlighted text</mark>  |  -                                                               |
|  Keyboard input  |  -                         |  `<kbd> </kbd>`                |  <kbd>keyboard key</kbd>        |  To show keyboard shortcuts                                      |
|  Inline Code     |  `` `code` ``              |  `<code> </code>`              |  `monospace code`               |  Single backticks, or HTML `<code>` tag                          |
|  Sample Output   |  -                         |  `<samp> </samp>`              |  <samp>monospace text</samp>    |  Monospace plain text, like Terminal/Console output              |

:information_source: Combining styling is possible, using **bold** `** **` and _italic_ `_ _` together like this `**_text_**` results in ⟶ **_text_**

---
<br>


## Structure, Content and Hyperlinking
<br>

<!-- class="extended" for texts without <br> tag -->    
<!-- class="truncated" for texts with the <br> tag --> 

<table align="center">
<!-------------------->
<!--- TABLE HEADER --->
<!-------------------->
<thead>
    <tr>
        <th>Name</th>
        <th>Markdown syntax</th>
        <th>HTML syntax</th>
<!--         <th>Output</th> -->
    </tr>
</thead>
<!------------------>
<!--- TABLE BODY --->
<!------------------>
<tbody>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- HEADINGS ---- SECTION --------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td align="center"><b>HEADINGS</b></td>
    <td align="center"></td>
    <td align="center"></td>
<!--     <td align="center"></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ATX HEADINGS ------------------------------------------------------------>
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">ATX<br>Headings</td>
    <!-- Markdown -->
    <td>
<pre lang="html">
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
</pre>
    </td>
    <!---- HTML ---->
    <td align="center">
<p class="extended">Headings can be centered with the attribute-value pair <code>align="center"</code></p>
<pre lang="html">
&lt;h1&gt;Heading 1&lt;/h1&gt;
&lt;h2&gt;Heading 2&lt;/h2&gt;
&lt;h3&gt;Heading 3&lt;/h3&gt;
&lt;h4&gt;Heading 4&lt;/h4&gt;
&lt;h5&gt;Heading 5&lt;/h5&gt;
&lt;h6&gt;Heading 6&lt;/h6&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- SETEXT HEADINGS --------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Setext<br>Headings</td>
    <!-- Markdown -->
    <td align="center">
<pre lang="html">
Heading 1
=========
Heading 2
---------
</pre>
    </td>
    <!---- HTML ---->
    <td align="center">
<pre lang="html">
&lt;h1&gt;Heading 1&lt;/h1&gt;
&lt;h2&gt;Heading 2&lt;/h2&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- HORIZONTAL LINE --------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Horizontal<br>Line</td>
    <!-- Markdown -->
    <td align="center">
<pre lang="markdown">
---
***
___
</pre>
    </td>
    <!---- HTML ---->
    <td align="center">
<pre lang="html">
&lt;hr&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- INFORMATIONAL BLOCKS ---- SECTION --------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td align="center"><b>INFORMATION<br>BLOCKS</b></td>
    <td align="center"></td>
    <td align="center"></td>
<!--     <td align="center"></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ALERTS ------------------------------------------------------------------>
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Alerts<br>ℹ️⚠️🔔❗</td>
    <!-- Markdown -->
    <td>
<pre lang="html">> [!NOTE]
> This is a note.</pre>
<pre lang="html">> [!WARNING]
> Warning message.</pre>
<pre lang="html">> [!IMPORTANT]
> Important message.</pre>
<pre lang="html">> [!CAUTION]
> Be careful.</pre>
    </td>
    <!---- HTML ---->
    <td align="center">-</td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- QUOTE BLOCK ------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Quote<br>block</td>
    <!-- Markdown -->
    <td>
<pre lang="html">
> This is a quote
> 
> It can span multiple lines</pre>
    </td>
    <!---- HTML ---->
    <td>
<pre lang="html">
&lt;blockquote&gt;
    &lt;p&gt;Quoted text.&lt;/p&gt;
&lt;/blockquote&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- MAIN CONTENT BLOCKS ---- SECTION ---------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td align="center"><b>MAIN<br>CONTENT<br>BLOCKS</b></td>
    <td align="center"></td>
    <td align="center"></td>
<!--     <td align="center"></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- PARAGRAPHS -------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Paragraphs</td>
    <!-- Markdown -->
    <td>
<pre lang="html">
First paragraph.
&lt;!-- blank line separation --&gt;
Second paragraph.
</pre>
    </td>
    <!---- HTML ---->
    <td>
<pre lang="html">
&lt;p&gt;One paragraph.&lt;/p&gt;
&lt;p&gt;Another paragraph.&lt;/p&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- COLLAPSED SECTION ------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Collapsed<br>Section</td>
    <!-- Markdown -->
    <td align="center">-</td>
    <!---- HTML ---->
    <td>
<p align="center">Requires a blank line after<br>the <code>&lt;summary&gt;</code> tag for markdown<br>to render properly</p>
<pre lang="html">
&lt;details&gt;
  &lt;summary&gt;Title&lt;/summary&gt;
  &lt;!-- blank line --&gt;
  Collapsed content.
&lt;/details&gt;</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- TABLES ------------------------------------------------------------------>
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Tables</td>
    <!-- Markdown -->
    <td>
<pre lang="markdown">
| Header A | Header B | Header C |
| -------- | :------: | -------: |
| a1       | b1       | c1       |
| default  | center   | right    |
</pre>
    </td>
    <!---- HTML ---->
    <td>
<pre lang="html">
&lt;table&gt;
    &lt;thead&gt;
        &lt;tr&gt;
            &lt;th&gt;A&lt;/th&gt;
            &lt;th&gt;B&lt;/th&gt;
        &lt;/tr&gt;
    &lt;/thead&gt;
    &lt;tbody&gt;
        &lt;tr&gt;
            &lt;td&gt;a1&lt;/td&gt;
            &lt;td&gt;b1&lt;/td&gt;
        &lt;/tr&gt;
    &lt;/tbody&gt;
&lt;/table&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- CODE BLOCK -------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Code<br>block</td>
    <!-- Markdown -->
    <td>
<pre lang="markdown">
```markdown
At least 3 backtick
characters (`) or
tildes (~).
You can choose syntax
highlighting on top
(check GitHub specs).
You have to match the
symbols on the bottom.
```
</pre>
<pre lang="markdown">
    4 spaces indentation
    in all lines of the 
    chosen code or text
    also creates a Code
    block in GFM.
</pre>
    </td>
    <!---- HTML ---->
    <td>
<pre lang="html">
&lt;pre&gt;&lt;code&gt;This code
will become a
Code block.
&lt;/code>&lt;/pre&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- DIAGRAMS ---------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Diagrams</td>
    <!-- Markdown -->
    <td>
<pre lang="markdown">
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
</pre>
    </td>
    <!---- HTML ---->
    <td align="center">-</td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- LIST TYPES ---- SECTION ------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td align="center"><b>LIST<br>TYPES</b></td>
    <td align="center"></td>
    <td align="center"></td>
<!--     <td align="center"></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- UNORDERED LIST ---------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Unordered<br>list</td>
    <!-- Markdown -->
    <td>
<pre lang="markdown">
+ List item
  + 1st level nesting
    + 2nd level nesting
+ Allows `+`, `-` or `*`
</pre>  
<pre lang="markdown">
* Combining symbols
- Creates some
+ Spacing
</pre>   
    </td>
    <!---- HTML ---->
    <td>
<pre lang="html">
&lt;ul&gt;
  &lt;li&gt;1st item&lt;/li&gt;
  &lt;li&gt;2nd item
    &lt;ul&gt;
      &lt;li&gt;1st nesting
        &lt;ul&gt;
          &lt;li&gt;2nd nesting&lt;/li&gt;
        &lt;/ul&gt;
      &lt;/li&gt;
    &lt;/ul&gt;
  &lt;/li&gt;
  &lt;li&gt;3rd item&lt;/li&gt;
&lt;/ul&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ORDERED LIST ------------------------------------------------------------>
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Ordered<br></r>list</td>
    <!-- Markdown -->
    <td>
<pre lang="markdown">
1. First item
2. Second item
   1. Nested item
      1. 2nd level nesting
7. Third item
&lt;!-- last one renders "3." --&gt;
</pre>
<pre lang="markdown">
1) You can also use:
   1) ")" instead of "."
2) Nesting:
    1) Must start with "1"
    2) "1." or "1)"
    3) for it to work
    4) And below starting
    5) letter of previous
    5) parent item
3. These ones won't apply nesting:
   3. Does not start with 1
  1. Does not indent correctly
</pre>
<pre lang="markdown">
1. Combining symbols
2) Creates some
3. Spacing
</pre>
    </td>
    <!---- HTML ---->
    <td>
<pre lang="html">
&lt;ol&gt;
  &lt;li&gt;1st item&lt;/li&gt;
  &lt;li&gt;2nd item
    &lt;ol&gt;
      &lt;li&gt;1st nesting
        &lt;ol&gt;
          &lt;li&gt;2nd nesting&lt;/li&gt;
        &lt;/ol&gt;
      &lt;/li&gt;
    &lt;/ol&gt;
  &lt;/li&gt;
  &lt;li&gt;3rd item&lt;/li&gt;
&lt;/ol&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- TASK LIST --------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Task<br>list</td>
    <!-- Markdown -->
    <td>
<p align="center"><a href="https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists">(1) GitHub Docs</a></p>
<p align="center"><a href="https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/about-task-lists">(2) GitHub Docs</a></p>
<pre lang="markdown">
- [ ] Incomplete task
- [x] Completed task
</pre>
    </td>
    <!---- HTML ---->
    <td align="center">-</td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- HYPERLINKS ---- SECTION ------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td align="center"><b>HYPERLINKS</b></td>
    <td align="center"></td>
    <td align="center"></td>
<!--     <td align="center"></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- AUTOLINK ---------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Autolink</td>
    <!-- Markdown -->
    <td align="center">
        <p>Needs a valid URL starting<br>with <code>http://</code> or <code>https://</code></p>
        <pre lang="markdown">https://github.com</pre>
    </td>
    <!---- HTML ---->
    <td align="center" class="extended"> Valid URLs are automatically converted to links</td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- HYPERLINK SYNTAX -------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Hyperlink<br>syntax</td>
    <!-- Markdown -->
    <td align="center">
        <p>Needs a valid URL starting<br>with <code>http://</code> or <code>https://</code></p>
        <p>Otherwise it will try to<br>reach relative paths<br>in your own repository<br>(e.g. <code>google.com</code>)</p>
        <pre lang="markdown">[anchor_text](https://URL)</pre>
    </td>
    <!---- HTML ---->
    <td>
<pre lang="html">
&lt;a href="valid_URL"&gt;Anchor text&lt;/a&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- LINKS BY ID ------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Links<br>by ID</td>
    <!-- Markdown -->
    <td align="center">
<p><a href="https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#custom-anchors">GitHub Docs</a></p>
<p>Headings get links automatically<br>generated, you can get their <code>#id</code><br>by hovering over them</p>
<pre lang="markdown">[linked text](#heading-id)</pre>
    </td>
    <!---- HTML ---->
    <td>
<p align="center">But in HTML you can create<br>your own with the <code>name=""</code> attribute</p>
<pre lang="html">
&lt;p name="name_id"&gt;Referenced text&lt;/a&gt;
<!-- blank space for better readability -->
&lt;a href="#name_id"&gt;text&lt;/a&gt;
</pre>
<p align="center">Or with the <code>id=""</code> attribute</p>
<pre lang="html">
&lt;p id="new_id"&gt;Referenced text&lt;/a&gt;
<!-- blank space for better readability -->
&lt;a href="#new_id"&gt;text&lt;/a&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- FILE LINKS -------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">File<br>Links</td>
    <!-- Markdown -->
    <td>
<p align="center">Relative paths within your<br>repository (follows <a href="https://en.wikipedia.org/wiki/Path_(computing)">Unix path syntax<a/>)</p>
<pre lang="markdown">
[Readme](./README.md)
[Config](../config/file.yml)
</pre>
    </td>
    <!---- HTML ---->
    <td>
<p align="center">Links are repository-relative<br>and work across branches</p>
<pre lang="html">
&lt;a href="./README.md"&gt;Read here&lt;/a&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!-----MENTION LINKS ------------------------------------------------------------>
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Mentions<br>links</td>
    <!-- Markdown -->
    <td>
<p align="center">ℹ️ Only works in comments</p>
<p>Mention users</p>
<pre lang="markdown">@username</pre>
<p>Mention Issues or PRs</p>
<pre lang="markdown">#123</pre>
    </td>
    <!---- HTML ---->
    <td align="center">-</td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- FOOTNOTES --------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Footnotes</td>
    <!-- Markdown -->
    <td>
<p align="center"><a href="https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#footnotes">GitHub Docs</a></p>
<pre lang="markdown">
Footnote reference[^1].
<!-- blank space -->
[^1]: Referenced text.
</pre>
    </td>
    <!---- HTML ---->
    <td align="center">-</td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- IMAGES ------------------------------------------------------------------>
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Images</td>
    <!-- Markdown -->
    <td>
<p align="center"><a href="https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#images">GitHub Docs</a></p>
<p align="center"><a href="https://github.github.com/gfm/#images">GFM Specs</a></p>
<p align="center"><a href="https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#uploading-assets">(drag and drop)</a></p>
<pre lang="markdown">
![Alt text](URL)
<!-- blank line -->
![Logo](./images/logo.png)
</pre>
    </td>
    <!---- HTML ---->
    <td>
<!-- <p align="center" class="truncated">The image can be centered by enclosing<br>it in a <code>p</code> tag and using the<br>attribute-value<br>pair <code>align="center"</code></p> -->
<p align="center" class="extended">The image can be centered by enclosing it in a <code>p</code> tag and using the attribute-value pair <code>align="center"</code></p>
<pre lang="html">
&lt;img src="URLorPATH" alt="text"&gt;
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- EDITING EXTRAS ---- SECTION --------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td align="center"><b>EDITING<br>EXTRAS</b></td>
    <td align="center"></td>
    <td align="center"></td>
<!--     <td align="center"></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ===== ------------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <td></td>
    <td></td>
    <td></td>
<!--    <td></td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- LINE BREAKS ------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Line<br>breaks</td>
    <!-- Markdown -->
    <td>
<p align="center"><a href="https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#line-breaks">GitHub Docs</a></p>
<p align="center">GitHub will render line breaks automatically<br>while editing (pressing <kbd>Enter</kbd>) in<br>issues, pull requests, or discussions<br>in a repository</p>
<p>Use 2 <kbd>spaces</kbd>:</p>
<pre>End a line with two spaces··
to create a line break.</pre>
<p>Or use a <code>\</code>:</p>
<pre>This is one line\
This is another line.</pre>
    </td>
    <!---- HTML ---->
    <td>
<p>Use the <code>&lt;br&gt;</code> self-closing tag:</p>
<pre lang="html">
This is one line&lt;br&gt;
This is another line.
</pre>
<p>As many as you want:</p>
<pre lang="html">
There will be&lt;br&gt;&lt;br&gt;&lt;br&gt;
3 line breaks.
</pre>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- ESCAPING ---------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Escaping<br>or ignoring<br>Markdown</td>
    <!-- Markdown -->
    <td>
<p align="center"><a href="https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#ignoring-markdown-formatting">GitHub Docs</a></p>
<p align="center"><a href="https://daringfireball.net/projects/markdown/syntax#backslash">original Specs</a></p>
<br>
<p align="center" class="extended">You can escape (ignore) certain Markdown reserved characters with <code>\</code> right before the character</p>
<br>
<p>Characters that can be escaped</p>
<pre lang="markdown">
\   backslash
`   backtick
*   asterisk
_   underscore
{}  curly braces
[]  square brackets
()  parentheses
#   hash mark
+   plus sign
-   minus sign (hyphen)
.   dot
!   exclamation mark
</pre>
<br>
<p>Ignores <i>italics</i> styling:</p>
<pre lang="markdown">
\*enclosed by asterisks\*
</pre>
<br>
<p>Ignores <code>inline code</code> styling:</p>
<pre lang="markdown">
\`enclosed by backticks\`
</pre>
    </td>
    <!---- HTML ---->
    <td align="center">-</td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- COMMENTS ---------------------------------------------------------------->
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Comments</td>
    <!-- Markdown -->
    <td>
<p align="center">GFM supports<br>HTML comments</p>
 <br>
<pre lang="markdown">
&lt;!-- This is a comment --&gt;
</pre>
    </td>
    <!---- HTML ---->
    <td>
 <br>
<pre lang="html">&lt;!-- Single line comment --&gt;</pre>
 <br>
<pre lang="html">
&lt;!--
Multiple
lines
comment
--&gt;
</pre>
 <br>
    </td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
<!------------------------------------------------------------------------------->
<!----- EMOJIS ------------------------------------------------------------------>
<!------------------------------------------------------------------------------->
<tr>
    <!---- Name ---->
    <td align="center">Emojis</td>
    <!-- Markdown -->
    <td>
<p align="center"><a href="https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#using-emojis">GitHub Docs</a></p>
<p align="center"><a href="https://github.com/ikatyang/emoji-cheat-sheet">Emoji Cheat Sheet</a></p>
<br>
<p align="center" class="extended">According to GitHub:<br><br><i>"Typing <kbd>:</kbd> will bring up a list of suggested emoji. The list will filter as you type, so once you find the emoji you're looking for, press <kbd>Tab</kbd> or <kbd>Enter</kbd> to complete the <mark>highlighted</mark> result."</i></p>
<br>
<p>This Mardown syntax:</p>
<pre lang="markdown">
:smile: :heart: :rocket:
</pre>
<p>Will render as:</p>
<pre>😄 ❤️ 🚀</pre>
    </td>
    <!---- HTML ---->
    <td align="center">-</td>
    <!--- Output --->
<!--     <td align="center">
        <p><a href="#">⬇️</a></p>
    </td> -->
</tr>
    </tbody>
</table>

    
