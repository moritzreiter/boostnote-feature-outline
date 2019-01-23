---
layout: default
---

# Text Formatting

Boostnote has advanced formatting options, some of them in form of Markdown
extensions that are not part of the standardized CommonMark specification. Those
formatting options that go beyond basic Markdown are listed here.

## Blocks

This section collates all formatting options that are rendered in some kind of
block and are not part of the CommonMark standard.

### Definitions

### Folding Blocks

### Generic Blocks

You can render text as a block with a border by indenting the content of the
block with a tab:

_Code:_

```;
↦I'm inside a
↦block with a border.
```

_Preview:_

![Block example](/assets/img/block.png)

Note that this only works if you set the _Editor Indent Style_ in Boostnote's
Interface Preferences to _Tab_, which unfortunately makes this feature a lot
less useful to you if you are on the good side of the Epic Tabs vs. Spaces
Chasm.

### Indications

### Tables

## To-do Checkboxes

## References

### Footnotes

### Tool tips

You can add tool tips to any phrase used in a note. The explanation will pop up
as a tool tip when hovering over the phrase and all occurrences of the phrase
itself will be decorated with a subtle dashed line. This is handy, for example,
to provide an explanation for abbreviations, as exemplified with the following
small excerpt from the website of the [The Dozenal Society of Great
Britain](http://www.dozenalsociety.org.uk).

_Code:_

```;
The DSGB [...] (founded 1959) and the DSA [...] (founded 1944) are separate
organisations with a common aim: to draw attention to the advantages of the
Dozen (or twelve-based) system for numeration and measurement.

*[DSGB]: The Dozenal Society of Great Britain
*[DSA]: The Dozenal Society of America
```

_Result:_

![Tooltip rendering example](/assets/img/tooltip.png)

## Substitutions

### Arrows

### Emoticons

### Keyboard Symbols

### Subscript & Superscript

_Code:_

```;
Drinking the 37^th^ cup of coffee on one day might cause a C~8~H~10~N~4~O~2~
overdose.
```

_Preview:_

![Subscript & superscript rendering example](/assets/img/subscript-and-superscript.png)
