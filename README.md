<!DOCTYPE html>
<html>
<head>
<title>mark-down-cheat-sheet.md</title>
<meta http-equiv="Content-type" content="text/html;charset=UTF-8">

<style>
/* https://github.com/microsoft/vscode/blob/master/extensions/markdown-language-features/media/markdown.css */
/*---------------------------------------------------------------------------------------------
 *  Copyright (c) Microsoft Corporation. All rights reserved.
 *  Licensed under the MIT License. See License.txt in the project root for license information.
 *--------------------------------------------------------------------------------------------*/

body {
	font-family: var(--vscode-markdown-font-family, -apple-system, BlinkMacSystemFont, "Segoe WPC", "Segoe UI", "Ubuntu", "Droid Sans", sans-serif);
	font-size: var(--vscode-markdown-font-size, 14px);
	padding: 0 26px;
	line-height: var(--vscode-markdown-line-height, 22px);
	word-wrap: break-word;
}

#code-csp-warning {
	position: fixed;
	top: 0;
	right: 0;
	color: white;
	margin: 16px;
	text-align: center;
	font-size: 12px;
	font-family: sans-serif;
	background-color:#444444;
	cursor: pointer;
	padding: 6px;
	box-shadow: 1px 1px 1px rgba(0,0,0,.25);
}

#code-csp-warning:hover {
	text-decoration: none;
	background-color:#007acc;
	box-shadow: 2px 2px 2px rgba(0,0,0,.25);
}

body.scrollBeyondLastLine {
	margin-bottom: calc(100vh - 22px);
}

body.showEditorSelection .code-line {
	position: relative;
}

body.showEditorSelection .code-active-line:before,
body.showEditorSelection .code-line:hover:before {
	content: "";
	display: block;
	position: absolute;
	top: 0;
	left: -12px;
	height: 100%;
}

body.showEditorSelection li.code-active-line:before,
body.showEditorSelection li.code-line:hover:before {
	left: -30px;
}

.vscode-light.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(0, 0, 0, 0.15);
}

.vscode-light.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(0, 0, 0, 0.40);
}

.vscode-light.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

.vscode-dark.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(255, 255, 255, 0.4);
}

.vscode-dark.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(255, 255, 255, 0.60);
}

.vscode-dark.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

.vscode-high-contrast.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(255, 160, 0, 0.7);
}

.vscode-high-contrast.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(255, 160, 0, 1);
}

.vscode-high-contrast.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

img {
	max-width: 100%;
	max-height: 100%;
}

a {
	text-decoration: none;
}

a:hover {
	text-decoration: underline;
}

a:focus,
input:focus,
select:focus,
textarea:focus {
	outline: 1px solid -webkit-focus-ring-color;
	outline-offset: -1px;
}

hr {
	border: 0;
	height: 2px;
	border-bottom: 2px solid;
}

h1 {
	padding-bottom: 0.3em;
	line-height: 1.2;
	border-bottom-width: 1px;
	border-bottom-style: solid;
}

h1, h2, h3 {
	font-weight: normal;
}

table {
	border-collapse: collapse;
}

table > thead > tr > th {
	text-align: left;
	border-bottom: 1px solid;
}

table > thead > tr > th,
table > thead > tr > td,
table > tbody > tr > th,
table > tbody > tr > td {
	padding: 5px 10px;
}

table > tbody > tr + tr > td {
	border-top: 1px solid;
}

blockquote {
	margin: 0 7px 0 5px;
	padding: 0 16px 0 10px;
	border-left-width: 5px;
	border-left-style: solid;
}

code {
	font-family: Menlo, Monaco, Consolas, "Droid Sans Mono", "Courier New", monospace, "Droid Sans Fallback";
	font-size: 1em;
	line-height: 1.357em;
}

body.wordWrap pre {
	white-space: pre-wrap;
}

pre:not(.hljs),
pre.hljs code > div {
	padding: 16px;
	border-radius: 3px;
	overflow: auto;
}

pre code {
	color: var(--vscode-editor-foreground);
	tab-size: 4;
}

/** Theming */

.vscode-light pre {
	background-color: rgba(220, 220, 220, 0.4);
}

.vscode-dark pre {
	background-color: rgba(10, 10, 10, 0.4);
}

.vscode-high-contrast pre {
	background-color: rgb(0, 0, 0);
}

.vscode-high-contrast h1 {
	border-color: rgb(0, 0, 0);
}

.vscode-light table > thead > tr > th {
	border-color: rgba(0, 0, 0, 0.69);
}

.vscode-dark table > thead > tr > th {
	border-color: rgba(255, 255, 255, 0.69);
}

.vscode-light h1,
.vscode-light hr,
.vscode-light table > tbody > tr + tr > td {
	border-color: rgba(0, 0, 0, 0.18);
}

.vscode-dark h1,
.vscode-dark hr,
.vscode-dark table > tbody > tr + tr > td {
	border-color: rgba(255, 255, 255, 0.18);
}

</style>

<style>
/* Tomorrow Theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */
/* Original theme - https://github.com/chriskempson/tomorrow-theme */

/* Tomorrow Comment */
.hljs-comment,
.hljs-quote {
	color: #8e908c;
}

/* Tomorrow Red */
.hljs-variable,
.hljs-template-variable,
.hljs-tag,
.hljs-name,
.hljs-selector-id,
.hljs-selector-class,
.hljs-regexp,
.hljs-deletion {
	color: #c82829;
}

/* Tomorrow Orange */
.hljs-number,
.hljs-built_in,
.hljs-builtin-name,
.hljs-literal,
.hljs-type,
.hljs-params,
.hljs-meta,
.hljs-link {
	color: #f5871f;
}

/* Tomorrow Yellow */
.hljs-attribute {
	color: #eab700;
}

/* Tomorrow Green */
.hljs-string,
.hljs-symbol,
.hljs-bullet,
.hljs-addition {
	color: #718c00;
}

/* Tomorrow Blue */
.hljs-title,
.hljs-section {
	color: #4271ae;
}

/* Tomorrow Purple */
.hljs-keyword,
.hljs-selector-tag {
	color: #8959a8;
}

.hljs {
	display: block;
	overflow-x: auto;
	color: #4d4d4c;
	padding: 0.5em;
}

.hljs-emphasis {
	font-style: italic;
}

.hljs-strong {
	font-weight: bold;
}
</style>

<style>
/*
 * Markdown PDF CSS
 */

 body {
	font-family: -apple-system, BlinkMacSystemFont, "Segoe WPC", "Segoe UI", "Ubuntu", "Droid Sans", sans-serif, "Meiryo";
	padding: 0 12px;
}

pre {
	background-color: #f8f8f8;
	border: 1px solid #cccccc;
	border-radius: 3px;
	overflow-x: auto;
	white-space: pre-wrap;
	overflow-wrap: break-word;
}

pre:not(.hljs) {
	padding: 23px;
	line-height: 19px;
}

blockquote {
	background: rgba(127, 127, 127, 0.1);
	border-color: rgba(0, 122, 204, 0.5);
}

.emoji {
	height: 1.4em;
}

code {
	font-size: 14px;
	line-height: 19px;
}

/* for inline code */
:not(pre):not(.hljs) > code {
	color: #C9AE75; /* Change the old color so it seems less like an error */
	font-size: inherit;
}

/* Page Break : use <div class="page"/> to insert page break
-------------------------------------------------------- */
.page {
	page-break-after: always;
}

</style>

<script src="https://unpkg.com/mermaid/dist/mermaid.min.js"></script>
</head>
<body>
  <script>
    mermaid.initialize({
      startOnLoad: true,
      theme: document.body.classList.contains('vscode-dark') || document.body.classList.contains('vscode-high-contrast')
          ? 'dark'
          : 'default'
    });
  </script>
<h1 id="1--headings">1- Headings</h1>
<p>How to give headings in Markdown file?</p>
<h1 id="heading-1">Heading 1</h1>
<h2 id="heading-2">Heading 2</h2>
<h3 id="heading-3">Heading 3</h3>
<h4 id="heading-4">Heading 4</h4>
<h5 id="so-on">so on</h5>
<h1 id="2--block-of-words">2- Block of words</h1>
<p>This is a normal text in markdown</p>
<blockquote>
<p>This a block of special text</p>
</blockquote>
<blockquote>
<p>This is second line of special text</p>
</blockquote>
<h1 id="3-line-break">3-Line Break</h1>
<p>This is a course with Baba Ammar python ka chilla 2024
in Data Science longwith python to do it in easiest way here apply all.<br>
This is second line</p>
<h1 id="4-combine-2-things">4-combine 2 things</h1>
<p>Block of words and heading</p>
<blockquote>
<p>** Heading 2</p>
</blockquote>
<h1 id="5-face-of-text">5 face of text.</h1>
<p><strong>Bold</strong></p>
<p><em>Italic</em></p>
<p><em><strong>Bold and Italic</strong></em></p>
<p>or u can use symbols
1- use of UnderScore(_)
<strong>Bold</strong></p>
<p><em>Italic</em></p>
<p><em><strong>Bold and Italic</strong></em></p>
<h1 id="6--bullet-points-or-lists">6- Bullet points or Lists</h1>
<blockquote>
<p>By Dash</p>
</blockquote>
<ul>
<li>
<p>Day-1</p>
</li>
<li>
<p>Day-2</p>
</li>
<li>
<p>Day-3</p>
</li>
<li>
<p>Day-4
-Day-5          Guess the error why dot is not shown here</p>
<ul>
<li>Day-5 a</li>
<li>Day-5 b
_ Sub-list (anything you want to mention here)</li>
<li>Day-5 c</li>
</ul>
</li>
<li>
<p>Day-6</p>
</li>
<li>
<p>Day-7</p>
<blockquote>
<p><strong>** Also by Using ( * or + )**</strong> as stearic already used twice.</p>
</blockquote>
</li>
</ul>
<ul>
<li>One</li>
<li>Day2
<ul>
<li>Day-2a</li>
<li>Day-2b</li>
</ul>
</li>
</ul>
<ul>
<li>Day-1</li>
<li>Day-2</li>
<li>Day-3
<ul>
<li>Day-3a</li>
<li>Day-3b</li>
</ul>
</li>
</ul>
<blockquote>
<p>Numbering of Lists</p>
</blockquote>
<ol>
<li>Day-1</li>
<li>Day-2</li>
<li>Day-3</li>
<li>Day-4 (Markdown understand the errors and mistakes)</li>
<li>Day-5
<ol>
<li>Day-5a</li>
<li>Day-5b</li>
<li>Day-5c</li>
</ol>
</li>
<li>Day-6</li>
</ol>
<h1 id="7--line-breaks-or-page-breaks">7- Line Breaks or Page Breaks</h1>
<p>This is line-1
This is Line-2
if after fullstop put an enter the line breaks
This is line-1.</p>
<p>This is Line-2.</p>
 <!-- if we want a line b/w these two then put 3-dash or 3_ Underscores or 3 stearics* -->
<h2 id="this-is-line-1">This is line-1.</h2>
<p>This is Line-2.</p>
<p>or</p>
<h2 id="this-is-line-1">This is line-1.</h2>
<hr>
<hr>
<p>This is Line-2.</p>
<h1 id="8-links-and-hyper-links">8-Links and Hyper-links</h1>
<p><a href="https://codanics.com/courses/python-ka-chilla-2024/lesson/markdown-language-in-72-minutes/">https://codanics.com/courses/python-ka-chilla-2024/lesson/markdown-language-in-72-minutes/</a></p>
<p><a href="https://codanics.com/courses/python-ka-chilla-2024/lesson/markdown-language-in-72-minutes/">The playlist for the markdown language is here.</a></p>
<p>and if we want to save link in a proper place</p>
<p>To see the markdown course <a href="https://codanics.com/courses/python-ka-chilla-2024/lesson/markdown-language-in-72-minutes/">here</a></p>
<h1 id="9-images-and-figures-with-links">9-Images and Figures with Links</h1>
<p>In order to use Wikipedia please scan thE following QR:
<img src="QR.svg" alt="QR">
or
<a href="QR.svg">QR</a></p>
<!-- > How to comment out markdown file and its short-cuts? -->
<p>For online pictures</p>
<p><a href="https://www.google.com/search?sca_esv=0a650f077e31c052&amp;sxsrf=ADLYWIKFAIfA-WCZ4kgM79jMKwgwPtyl8A:1728405275775&amp;q=codonics+codanics&amp;uds=ADvngMjcH0KdF7qGWtwTBrP0nt7d5Va50E0UzczXq8yL5f8lNfdAgjMd4-W2K4O4i8YeUoe6WAA310lCzEmJfS-yoCAsqCnh7R1CJaNuw9tYq7jIRG1HTPm6xu5xAVoXFlSqQkyNZ9lfgB_uLpIms2C92ofqm_Ukqg&amp;udm=2&amp;sa=X&amp;ved=2ahUKEwiX5vWzm_-IAxUWcvEDHQWCGyMQxKsJegQICBAB&amp;ictx=0&amp;biw=1366&amp;bih=607&amp;dpr=1#vhid=TmO8iB8bjolieM&amp;vssid=mosaic">Codanics</a></p>
<p>if you want to show a picture here alongwith the wordings then  put the sign!</p>
<p><img src="https://www.google.com/search?sca_esv=0a650f077e31c052&amp;sxsrf=ADLYWIKFAIfA-WCZ4kgM79jMKwgwPtyl8A:1728405275775&amp;q=codonics+codanics&amp;uds=ADvngMjcH0KdF7qGWtwTBrP0nt7d5Va50E0UzczXq8yL5f8lNfdAgjMd4-W2K4O4i8YeUoe6WAA310lCzEmJfS-yoCAsqCnh7R1CJaNuw9tYq7jIRG1HTPm6xu5xAVoXFlSqQkyNZ9lfgB_uLpIms2C92ofqm_Ukqg&amp;udm=2&amp;sa=X&amp;ved=2ahUKEwiX5vWzm_-IAxUWcvEDHQWCGyMQxKsJegQICBAB&amp;ictx=0&amp;biw=1366&amp;bih=607&amp;dpr=1#vhid=TmO8iB8bjolieM&amp;vssid=mosaic" alt="Codanics"></p>
<h1 id="10-adding-code-or-code-block">10-Adding Code or Code block</h1>
<p>To print a string use backticks present before 1
<code>print(&quot;hello&quot;)</code>
or</p>
<pre class="hljs"><code><div>
 print(&quot;Codanics&quot;)
</div></code></pre>
<pre class="hljs"><code><div>print(&quot;hello Mr.&quot;)
</div></code></pre>
<p>But also to add a block of code use this sign three times above and below and in b/w you have to write the code.</p>
<blockquote>
<p>The code will show color according to Python language syntax.</p>
</blockquote>
<pre class="hljs"><code><div>x = <span class="hljs-number">5</span>+<span class="hljs-number">6</span>
y = <span class="hljs-number">3</span><span class="hljs-number">-2</span>
z = x+y
print(z)

</div></code></pre>
<!-- if you use this you will have a copy option on the github
and if you mark the name of language it also show fonts of that language. as above for python.
> The code will show color according to R language syntax. -->
<pre class="hljs"><code><div>x = <span class="hljs-number">5</span>+<span class="hljs-number">6</span>
y = <span class="hljs-number">3</span>-<span class="hljs-number">2</span>
z = x+y
print(z)

</div></code></pre>
<h1 id="11-adding-tables">11-adding tables</h1>
<p>|(pipe) by clicking shift+button before the pg up button</p>
<table>
<thead>
<tr>
<th style="text-align:center">Species</th>
<th style="text-align:center">Petal-length</th>
<th style="text-align:center">Sepal-length</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center">Virginica</td>
<td style="text-align:center">15.1.2</td>
<td style="text-align:center">17.2</td>
</tr>
<tr>
<td style="text-align:center">Setosa</td>
<td style="text-align:center">18.2</td>
<td style="text-align:center">19.2</td>
</tr>
<tr>
<td style="text-align:center">Versicolor</td>
<td style="text-align:center">12.2</td>
<td style="text-align:center">12.2</td>
</tr>
<tr>
<td style="text-align:center">Virginica</td>
<td style="text-align:center">18.2</td>
<td style="text-align:center">19.2</td>
</tr>
<tr>
<td style="text-align:center">Virginica</td>
<td style="text-align:center">18.2</td>
<td style="text-align:center">19.2</td>
</tr>
<tr>
<td style="text-align:center">Setosa</td>
<td style="text-align:center">18.2</td>
<td style="text-align:center">19.2</td>
</tr>
</tbody>
</table>
<p>if a colon on right side as ! it will be right aligned. or if left it is aligned on left. and if middle align on both side mark ! but with no space</p>
<h1 id="12-contents">12-Contents</h1>
<p>just as link
sample text for paper contents</p>
<p><a href="#1--headings">1- Headings</a><br>
<a href="#2--block-of-words">2- Block-of-words/Citations</a><br>
<a href="#3-face-of-text">3- Face of Text</a><br>
<a href="#4-combine-2-things">4-combine 2 yt </a><br>
<a href="#5-face-of-text">5- Face OF TEXT</a><br>
<a href="#6--bullet-points-or-lists">6- Bullt-POINTS</a><br>
<a href="#7--line-breaks-or-page-breaks">7- Line Breaks</a><br>
<a href="#8-links-and-hyper-links">8- Links and Hyper-links</a><br>
<a href="#9-images-and-figures-with-links">9- Figures</a><br>
<a href="#10-adding-code-or-code-block">10 code-or-code blocks</a><br>
<a href="#11-adding-tables">11- Tables</a></p>
<h1 id="13-install-extensions">13-Install Extensions</h1>
<!-- if select and right clicking -->
<p><strong>simple text</strong></p>
<!-- or simply by ctrl+b -->
  <!-- Next by ctrl+i -->
<p><em>Italic</em></p>
 <!-- Next by shift+3times underscore -->
<p><em><strong>Italic and Bold</strong></em></p>
<!-- by selecting and right clicking toggle hyperlink -->
<p><a href="https://www.google.com/search?sca_esv=0a650f077e31c052&amp;sxsrf=ADLYWIKFAIfA-WCZ4kgM79jMKwgwPtyl8A:1728405275775&amp;q=codonics+codanics&amp;uds=ADvngMjcH0KdF7qGWtwTBrP0nt7d5Va50E0UzczXq8yL5f8lNfdAgjMd4-W2K4O4i8YeUoe6WAA310lCzEmJfS-yoCAsqCnh7R1CJaNuw9tYq7jIRG1HTPm6xu5xAVoXFlSqQkyNZ9lfgB_uLpIms2C92ofqm_Ukqg&amp;udm=2&amp;sa=X&amp;ved=2ahUKEwiX5vWzm_-IAxUWcvEDHQWCGyMQxKsJegQICBAB&amp;ictx=0&amp;biw=1366&amp;bih=607&amp;dpr=1#vhid=TmO8iB8bjolieM&amp;vssid=mosaic"> Link</a></p>
<p><img src="QR.svg" alt="Image"></p>
<pre class="hljs"><code><div>&gt;  image by citation 

</div></code></pre>
<p><s>image</s> by <code>strikethrough</code></p>
   <!-- by clicking on add tables -->
<table>
<thead>
<tr>
<th>Column A</th>
<th>Column B</th>
<th>Column C</th>
</tr>
</thead>
<tbody>
<tr>
<td>A1</td>
<td>B1</td>
<td>C1</td>
</tr>
<tr>
<td>A2</td>
<td>B2</td>
<td>C2</td>
</tr>
<tr>
<td>A3</td>
<td>B3</td>
<td>C3</td>
</tr>
</tbody>
</table>
<p>with header</p>
<table>
<thead>
<tr>
<th>Column A</th>
<th>Column B</th>
<th>Column C</th>
</tr>
</thead>
<tbody>
<tr>
<td>A1</td>
<td>B1</td>
<td>C1</td>
</tr>
<tr>
<td>A2</td>
<td>B2</td>
<td>C2</td>
</tr>
<tr>
<td>A3</td>
<td>B3</td>
<td>C3</td>
</tr>
</tbody>
</table>

</body>
</html>
