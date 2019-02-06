---
layout: default
---

# Chart.js

_Code:_

<!-- markdownlint-disable MD031 -->

```;
``​`chart(yaml)
type: pie
data:
  labels:
  - Internet Explorer
  - Netscape/Mozilla
  - Safari
  - Opera
  - Other
  datasets:
  - data:
    - 95.04
    - 2.37
    - 0.67
    - 0.51
    - 0.32
    backgroundColor:
    - "royalblue"
    - "darkorange"
    - "silver"
    - "crimson"
    - "gold"
    hoverBackgroundColor:
    - "lightsteelblue"
    - "lightsalmon"
    - "gainsboro"
    - "indianred"
    - "khaki"
``​​`
```

<!--
There's a Zero Width Space between two of the inner opening and closing three
backticks to prevent them from being interpreted as closing the outer opening
three backticks.
-->

<!-- markdownlint-enable MD013 -->

_Result:_

![Chart.js example](/assets/img/chartjs.png)

The chart shows the usage share of web browsers in Q2 2004 (Source:
[Wikipedia](https://en.wikipedia.org/wiki/Usage_share_of_web_browsers#TheCounter.com_(2000_to_2009))).
