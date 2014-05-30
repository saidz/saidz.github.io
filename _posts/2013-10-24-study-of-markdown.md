---
layout: post
title: study notes of markdown
description: "the original syntax of markdown"
categories: other
date: 2013-10-24
---
## synopsis
### goal
make wirting and reading more easy 
reading and writing a markdown file would like read a normal text file		
### syntax
syntax of markdown is a group of punctuation
### opinion
* not another html syntax ,just use a simple syntax to replace the usually html label
* make writing more easy
* the html label also can use in md file(there are some note)
***
## Inline HTML
when inline HTML at md file,the follow things you have to knows:

1. md was design to be a language for web content
It's not a another html syntax;In a md file you can insert html label that would be identified and parsed;
It's necessary to skip a line when some blocks element -`<div>`、`<table>`、`<pre>`、`<p>`,are insert to markdown.

	This is a regular paragraph.

	<table>
		<tr>
			<td>Foo</td>
		</tr>
	</table>

	This is another regular paragraph.

2.  md syntax is valid in inline label,invalid in block label
The markdown syntax in the HTML block label would not be parsed.
The inline label -`<span>`、`<cite>`、`<del>`, would be parsed.
* the follow md would not be parsed

<p>
**abc**
</p>
* the follow md would be parsed
<span>
**abc**
</span>
***
## special meta character
