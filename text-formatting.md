---
layout: default
---

# Text Formatting

Boostnote's advanced formatting options beyond basic Markdown (some of them are
non-standardized Markdown extensions) are listed in this category.

## Blocks

This section collates all formatting options that are rendered in some kind of
block and are not part of the CommonMark standard.

### Definitions

You can create definitions by having the term on one line by itself, following
by the definition text prefixed with a `:` or a `~`. Note that you can use
Markdown formatting in the definition text.

_Code:_

<!-- markdownlint-disable MD013 -->

```;
Cuneiform
: __Cuneiform__ or __Sumerian cuneiform__, one of the earliest systems of
writing, was invented by the Sumerians. It is distinguished by its wedge-shaped
marks on clay tablets, made by means of a blunt reed for a stylus.
The name _cuneiform_ itself simply means "wedge shaped".

Quipu
~ __Quipu__ (also spelled __khipu__), or __talking knots__, were recording
devices fashioned from strings historically used by a number of cultures in the
region of Andean South America.
```

<!-- markdownlint-enable MD013 -->

_Result:_

![Definitions example](/assets/img/definitions.png)

(Source: Wikipedia [1](https://en.wikipedia.org/wiki/Quipu),
[2](https://en.wikipedia.org/wiki/Cuneiform))

### Folding Blocks

_Code:_

```;
<details>
👹
</details>

<details>
<summary>
Ingredients
</summary>
1 part to 3 parts Gin (to taste)<br />
3 parts tonic water
</details>
```

_Result:_

![Folded folding block example](/assets/img/folding-block-folded.png)

![Unfolded folding block example](/assets/img/folding-block-unfolded.png)

### Indications

_Code:_

<!-- markdownlint-disable MD013 -->

```;
!!! note Note
What one programmer can do in one month, two programmers can do in two months.
(Fred Brooks)
!!!

!!! hint Hint
Deleted code is debugged code. (Jeff Sickel)
!!!

!!! caution Caution
Never trust a computer you can’t throw out a window. (Steve Wozniak)
!!!

!!! error Error
Should array indices start at 0 or 1? My compromise of 0.5 was rejected without,
I thought, proper consideration. (Stan Kelly-Bootle)
!!!

!!! attention Attention
Any code of your own that you haven't looked at for six or more months might as
well have been written by someone else. (Eagleson's law)
!!!

!!! danger Danger
Make sure that the old quote "they muddy the water so that it seems deep"
doesn't describe your engineering style/codebases. (Sarah Drasner)
!!!
```

<!-- markdownlint-enable MD013 -->

_Result:_

![Indications example](/assets/img/indications.png)

(Source: [@CodeWisdom](https://twitter.com/CodeWisdom))

### Tables

Tables (as well as [task list items](#task-list-items)) are a Markdown extension
in [GitHub Flavored Markdown](https://github.github.com/gfm/#tables-extension-).
Note how you can tweak alignment in cells by positioning a colon character at
either the left side, the right or both sides just under the header row for
left, right or center alignment respectively, left alignment being the default.

_Code:_

```;
| Programming Language | 2019 | 2014 | 2009 | 2004 | 1999 | 1994 | 1989 |
| :------------------: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| _Java_               | 1    | 2    | 1    | 1    | 14   |            ||
| _C_                  | 2    | 1    | 2    | 2    | 1    | 1    | 1    |
| _C++_                | 3    | 4    | 3    | 3    | 2    | 2    | 3    |
| _Python_             | 4    | 7    | 5    | 10   | 20   | 21   |      |
| _Visual Basic .NET_  | 5    | 11   |                              |||||
| _C#_                 | 6    | 5    | 7    | 8    | 30   |            ||
| _PHP_                | 7    | 6    | 4    | 5    |                  |||
| _JavaScript_         | 8    | 8    | 8    | 7    | 19   |            ||
| _SQL_                | 9    |            || 6    |                  |||
| _Ruby_               | 10   | 10   | 10   | 22   |                  |||
[TIOBE Very Long Term History Positions]
```

_Result:_

![Table example](/assets/img/table.png)

(Source: [TIOBE Index](https://www.tiobe.com/tiobe-index/))

## References

There are two types of references: footnotes and tooltips.

### Footnotes

_Code:_

<!-- markdownlint-disable MD013 -->

```;
> In mathematical terms, Lacan[^lacan] is here pointing out that the first
> homology group of the sphere is trivial, while those of the other surfaces are
> profound; and this homology is linked with the connectedness or
> disconnectedness of the surface after one or more cuts. Furthermore, as Lacan
> suspected, there is an intimate connection between the external structure of
> the physical world and its inner psychological representation qua knot theory:
> this hypothesis has recently been confirmed by Witten's derivation of knot
> invariants (in particular the Jones polynomial) from three-dimensional
> Chern-Simons quantum field theory.[^sokal]

[^lacan]: [Jacques Lacan - Wikipedia](https://en.wikipedia.org/wiki/Jacques_Lacan)
[^sokal]: Sokal, Alan D. 1996. “Transgressing the Boundaries: Towards a
```

_Result:_

<!-- markdownlint-enable MD013 -->

![Footnotes example](/assets/img/footnotes.png)

### Tool Tips

You can add tool tips to any phrase used in a note. The explanation will pop up
as a tool tip when hovering over the phrase and all occurrences of the phrase
itself will be decorated with a subtle dashed line. This is handy, for example,
to provide an explanation for abbreviations.

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

(Source: [The Dozenal Society of Great
Britain](http://www.dozenalsociety.org.uk))

## Various Substitutions

Here are some simple substitution features.

### Emojis

_Code:_

```;
:hamburger: :fries: :beer:
```

_Result:_

![Emoji example](/assets/img/emojis.png)

### Keyboard Symbols

_Code:_

```;
[[Ctrl]][[Alt]][[Delete]]
```

_Result:_

![Keyboard symbols example](/assets/img/keyboard-symbols.png)

### Subscript & Superscript

_Code:_

```;
Drinking the 37^th^ cup of coffee on one day might cause a C~8~H~10~N~4~O~2~ overdose.
```

_Result:_

![Subscript & superscript rendering example](/assets/img/subscript-and-superscript.png)

### Task List Items

Tast list items, just like [Tables](#tables), are a Markdown extension from
[GitHub Flavored
Markdown](https://github.github.com/gfm/#task-list-items-extension-). When a
note contains one or more task list items, Boostnote will show a progress bar on
top of the note reflecting the proportion of ticked to unticked items. This
effectively turns a note into a nice and simple project planner.

_Code:_

```;
- [x] Try
- [x] Fail
- [ ] Try again
- [ ] Fail better
```

_Result:_

![Task list items example](/assets/img/task-list-items.png)
