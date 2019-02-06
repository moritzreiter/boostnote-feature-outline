---
layout: default
---

# js-sequence-diagrams


_Code:_

<!-- markdownlint-disable MD031 -->

```;
`​``sequence
Andrew->China: Says Hello
Note right of China: China thinks\nabout it
China-->Andrew: How are you?
Andrew->>China: I am good thanks!
`​``
```

<!--
There's a Zero Width Space between two of the inner closing three backticks
to prevent them from being interpreted as closing the outer opening three
backticks.
-->

<!-- markdownlint-enable MD013 -->

_Result:_

![js-sequence-diagram example](/assets/img/sequence.png)

(Source: [js-sequence-diagrams](https://bramp.github.io/js-sequence-diagrams/))
