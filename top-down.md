```mermaid
graph LR
    Start --> Stop
```

```mermaid
graph TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
```

```mermaid
flowchart LR
  subgraph TOP
    direction TB
    subgraph B1
        direction RL
        i1 -->f1
    end
    subgraph B2
        direction BT
        i2 -->f2
    end
  end
  A --> TOP --> B
  B1 --> B2
```

```mermaid
  flowchart LR
      subgraph DB
      direction TB
        db[( )] --> X
      end
  A --> DB
```

[![](https://mermaid.ink/img/eyJjb2RlIjoiICBmbG93Y2hhcnQgTFJcbiAgICAgIHN1YmdyYXBoIERCXG4gICAgICBkaXJlY3Rpb24gVEJcbiAgICAgICAgZGJbKCApXSAtLT4gWFxuICAgICAgZW5kXG4gIEEgLS0-IERCXG4gIFxuIFxuIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZSwiYXV0b1N5bmMiOnRydWUsInVwZGF0ZURpYWdyYW0iOmZhbHNlfQ)](https://mermaid-js.github.io/mermaid-live-editor/edit/##eyJjb2RlIjoiICBmbG93Y2hhcnQgTFJcbiAgICAgIHN1YmdyYXBoIERCXG4gICAgICBkaXJlY3Rpb24gVEJcbiAgICAgICAgZGJbKCApXSAtLT4gWFxuICAgICAgZW5kXG4gIEEgLS0-IERCIFxuICBcbiBcbiIsIm1lcm1haWQiOiJ7XG4gIFwidGhlbWVcIjogXCJkZWZhdWx0XCJcbn0iLCJ1cGRhdGVFZGl0b3IiOmZhbHNlLCJhdXRvU3luYyI6dHJ1ZSwidXBkYXRlRGlhZ3JhbSI6ZmFsc2V9)

---

```mermaid
flowchart LR
  subgraph user
  direction LR
    a --> b
    b --> c
    c --> d
    d --> a
  end
  subgraph auto
  direction LR
    e --> f
    f --> g
    g --> h
  end
  user --> auto
   
```
[![](https://mermaid.ink/img/eyJjb2RlIjoiZmxvd2NoYXJ0IExSXG4gIHN1YmdyYXBoIHVzZXJcbiAgZGlyZWN0aW9uIExSXG4gICAgYSAtLT4gYlxuICAgIGIgLS0-IGNcbiAgICBjIC0tPiBkXG4gICAgZCAtLT4gYVxuICBlbmRcbiAgc3ViZ3JhcGggYXV0b1xuICBkaXJlY3Rpb24gTFJcbiAgICBlIC0tPiBmXG4gICAgZiAtLT4gZ1xuICAgIGcgLS0-IGhcbiAgZW5kXG4gIHVzZXIgLS0-IGF1dG9cbiAgXG4gXG4iLCJtZXJtYWlkIjp7InRoZW1lIjoiZGVmYXVsdCJ9LCJ1cGRhdGVFZGl0b3IiOmZhbHNlLCJhdXRvU3luYyI6dHJ1ZSwidXBkYXRlRGlhZ3JhbSI6ZmFsc2V9)](https://mermaid-js.github.io/mermaid-live-editor/edit/##eyJjb2RlIjoiZmxvd2NoYXJ0IExSXG4gIHN1YmdyYXBoIHVzZXJcbiAgZGlyZWN0aW9uIExSXG4gICAgYSAtLT4gYlxuICAgIGIgLS0-IGNcbiAgICBjIC0tPiBkXG4gICAgZCAtLT4gYVxuICBlbmRcbiAgc3ViZ3JhcGggYXV0b1xuICBkaXJlY3Rpb24gXG4gICAgZSAtLT4gZlxuICAgIGYgLS0-IGdcbiAgICBnIC0tPiBoXG4gIGVuZFxuICB1c2VyIC0tPiBhdXRvXG4gIFxuIFxuIiwibWVybWFpZCI6IntcbiAgXCJ0aGVtZVwiOiBcImRlZmF1bHRcIlxufSIsInVwZGF0ZUVkaXRvciI6ZmFsc2UsImF1dG9TeW5jIjp0cnVlLCJ1cGRhdGVEaWFncmFtIjpmYWxzZX0)

---

