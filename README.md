```mermaid
---
config:
  look: handDrawn
  securityLevel: antiscript
  flowchart:
    diagramPadding: 0
    nodeSpacing: 15
    rankSpacing: 50
    padding: 15
---
flowchart LR
    BLOG(blog)
    NPM(npm packages)
    CODE@{ shape: st-rect, label: "code smells"}
    A(SPOJ - Rust)
    B(🎄 AoC 21' - TypeScript)
    C(🎄 AoC 22' - Python)

    BLOG --- NPM --- CODE
    CODE --> A
    CODE --> B ~~~~ END
    CODE --> C

    click BLOG href "https://twistezo.github.io/blog/" _blank
    click NPM href "https://www.npmjs.com/~twistezo" _blank
    click A href "https://github.com/twistezo/spoj-tournament" _blank
    click B href "https://github.com/twistezo/advent-of-code-2021" _blank
    click C href "https://github.com/twistezo/advent-of-code-2021" _blank

    classDef hidden display: none
    class END hidden
    class BLOG,NPM,CODE,A,B,C link
    classDef link text-decoration: none
```
