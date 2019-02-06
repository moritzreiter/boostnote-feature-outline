---
layout: default
---

# mermaid

_Code:_

<!-- markdownlint-disable MD031 -->

```;
`​``mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->John: Hello John, how are you?
    loop Healthcheck
        John->John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->Alice: Great!
    John->Bob: How about you?
    Bob-->John: Jolly good!
`​`​`
```

<!--
There's a Zero Width Space between two of the inner closing three backticks
to prevent them from being interpreted as closing the outer opening three
backticks.
-->

<!-- markdownlint-enable MD013 -->

_Result:_

![Mermaid example](/assets/img/mermaid.png)

(Source: [mermaidjs.github.io](https://mermaidjs.github.io))
