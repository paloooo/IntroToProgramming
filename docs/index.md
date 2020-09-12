# Welcome
You should add your project description right here to let the user know what this page is actually for - in this case documentation.

!!! note
	This is an admonition which was spawned using:

	```md
	!!! note
		This is an admonition which was spawned using:
		...
	```

## Buttons

[This is a button](#){: .md-button }

```md
[This is a button](#){: .md-button }
```

[This is a button](#){: .md-button .md-button--primary }
```md
[This is a button](#){: .md-button .md-button--primary }
```

## Tabs

=== "CPython"

	``` python
	def output(input):
		print(input)

	output("hello world")
	```

=== "JavaScript"

	``` JS
	function output(input){
		console.log(input)
	}

	output("hello world")
	```

```md
=== "Header 1"

	Content goes here

=== "Header 2"

	content goes here
```

## Tables

| Item        | Description                          |
| ----------- | ------------------------------------ |
| Example 1   | Woah! an example?!                   |
| Example 2   | The second example that is here      |

```md
| Item        | Description                          |
| ----------- | ------------------------------------ |
| Example 1   | Woah! an example?!                   |
| Example 2   | The second example that is here      |

```

## Footnotes
hi[^1] this is a footnote link

[^1]:
 this is the footnote

```MD
hi[^1] this is a footnote link

[^1]:
 this is the footnote
```

## Formatting
### Bold

=== "Result"

	this is some **emphasised** text.

=== "Code"

	```md
	this is some **emphasised** text.
	```

### Italic

=== "Result"

	this is some _italicized_ text.

=== "Code"

	```md
	this is some _italicized_ text.
	```

### Line

=== "Result"

	~~Never meant to say this~~

=== "Code"

	```md
	~~Never meant to say this~~
	```

### Underline

=== "Result"

	^^No i really didn't mean to.^^

=== "Code"

	```md
	^^No i really didn't mean to.^^
	```

### Subscript

=== "Result"

	D~oes~ this ~look~ off?

=== "Code"

	```md
	D~oes~ this ~look~ off?
	```

### Subscript

=== "Result"

	W~e~ ^bet^ ~it~ ^does^.

=== "Code"

	```md
	W~e~ ^bet^ ~it~ ^does^.
	```

### Hightlight

=== "Result"

	==A piece of decoration - hightlighting is not used often.==

=== "Code"

	```md
	==A piece of decoration - hightlighting is not used often.==
	```


### Emojis

=== "Result"

	wow - emojis are fun! :smile:

=== "Code"

	```md
	wow - emojis are fun! :smile:
	```

### Checkboxes

=== "Result"

	* [x] this is a checkbox
	* [ ] this is also a checkbox

=== "Code"

	```md
	* [x] this is a checkbox
	* [ ] this is also a checkbox
	```
