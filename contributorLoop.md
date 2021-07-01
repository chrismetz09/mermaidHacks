
```mermaid
graph LR;
A-->B;
B-->C;
C-->D;
subgraph DB

db[(Your Fork of main<br>K8s )] --> Y    
end
D-->db[(Your Fork of main<br>K8s )];
subgraph REVIEW
flowchart TB
    X-->Y;
    X-->F
end
db-->REVIEW-->A

```

---

```mermaid
flowchart LR

  subgraph createContent
  direction LR
    a[(your<br>fork)] -- suggest<br>edits--> b[YOU]
    b <--> c[HUGO]
    c -- push commits --> a
  end
  subgraph DEPLOY
    direction LR
      e[(Main<br>K8s<br>repo)] --> f
      f[(Netlify<br>build<br>deploy)] --> g[(K8s.io)]
   end
  createContent -- merge --> DEPLOY
  subgraph Fork
        direction TB
        db[(Main<br>K8s<br>repo)] --> L[(your<br>fork)]
  end
      subgraph openPR
      direction LR
        M[YOU] --> N[(your<br>fork)]
    end
    subgraph forkMain 
      direction LR
      x[YOU] --> Fork
    end
```

[![](https://mermaid.ink/img/eyJjb2RlIjoiZmxvd2NoYXJ0IExSXG5cbiAgc3ViZ3JhcGggY3JlYXRlQ29udGVudFxuICBkaXJlY3Rpb24gTFJcbiAgICBhWyh5b3VyPGJyPmZvcmspXSAtLSBzdWdnZXN0PGJyPmVkaXRzLS0-IGJbWU9VXVxuICAgIGIgPC0tPiBjW0hVR09dXG4gICAgYyAtLSBwdXNoIGNvbW1pdHMgLS0-IGFcbiAgZW5kXG4gIHN1YmdyYXBoIERFUExPWVxuICAgIGRpcmVjdGlvbiBMUlxuICAgICAgZVsoTWFpbjxicj5LOHM8YnI-cmVwbyldIC0tPiBmXG4gICAgICBmWyhOZXRsaWZ5PGJyPmJ1aWxkPGJyPmRlcGxveSldIC0tPiBnWyhLOHMuaW8pXVxuICAgZW5kXG4gIGNyZWF0ZUNvbnRlbnQgLS0gbWVyZ2UgLS0-IERFUExPWVxuICBzdWJncmFwaCBGb3JrXG4gICAgICAgIGRpcmVjdGlvbiBUQlxuICAgICAgICBkYlsoTWFpbjxicj5LOHM8YnI-cmVwbyldIC0tPiBMWyh5b3VyPGJyPmZvcmspXVxuICBlbmRcbiAgICAgIHN1YmdyYXBoIG9wZW5QUlxuICAgICAgZGlyZWN0aW9uIExSXG4gICAgICAgIE1bWU9VXSAtLT4gTlsoeW91cjxicj5mb3JrKV1cbiAgICBlbmRcbiAgICBzdWJncmFwaCBmb3JrTWFpbiBcbiAgICAgIGRpcmVjdGlvbiBMUlxuICAgICAgeFtZT1VdIC0tPiBGb3JrXG4gICAgZW5kXG5cbiAgXG5cbiAgICBcbiAgXG4gXG4iLCJtZXJtYWlkIjp7InRoZW1lIjoiZGVmYXVsdCJ9LCJ1cGRhdGVFZGl0b3IiOmZhbHNlLCJhdXRvU3luYyI6dHJ1ZSwidXBkYXRlRGlhZ3JhbSI6ZmFsc2V9)](https://mermaid-js.github.io/mermaid-live-editor/edit/##eyJjb2RlIjoiZmxvd2NoYXJ0IExSXG5cbiAgc3ViZ3JhcGggY3JlYXRlQ29udGVuXG4gIGRpcmVjdGlvbiBMUlxuICAgIGFbKHlvdXI8YnI-Zm9yayldIC0tIHN1Z2dlc3Q8YnI-ZWRpdHMtLT4gYltZT1VdXG4gICAgYiA8LS0-IGNbSFVHT11cbiAgICBjIC0tIHB1c2ggY29tbWl0cyAtLT4gYVxuICBlbmRcbiAgc3ViZ3JhcGggREVQTE9ZXG4gICAgZGlyZWN0aW9uIExSXG4gICAgICBlWyhNYWluPGJyPks4czxicj5yZXBvKV0gLS0-IGZcbiAgICAgIGZbKE5ldGxpZnk8YnI-YnVpbGQ8YnI-ZGVwbG95KV0gLS0-IGdbKEs4cy5pbyldXG4gICBlbmRcbiAgY3JlYXRlQ29udGVudCAtLSBtZXJnZSAtLT4gREVQTE9ZXG4gIHN1YmdyYXBoIEZvcmtcbiAgICAgICAgZGlyZWN0aW9uIFRCXG4gICAgICAgIGRiWyhNYWluPGJyPks4czxicj5yZXBvKV0gLS0-IExbKHlvdXI8YnI-Zm9yayldXG4gIGVuZFxuICAgICAgc3ViZ3JhcGggb3BlblBSXG4gICAgICBkaXJlY3Rpb24gTFJcbiAgICAgICAgTVtZT1VdIC0tPiBOWyh5b3VyPGJyPmZvcmspXVxuICAgIGVuZFxuICAgIHN1YmdyYXBoIGZvcmtNYWluIFxuICAgICAgZGlyZWN0aW9uIExSXG4gICAgICB4W1lPVV0gLS0-IEZvcmtcbiAgICBlbmRcblxuICBcblxuICAgIFxuICBcbiBcbiIsIm1lcm1haWQiOiJ7XG4gIFwidGhlbWVcIjogXCJkZWZhdWx0XCJcbn0iLCJ1cGRhdGVFZGl0b3IiOmZhbHNlLCJhdXRvU3luYyI6dHJ1ZSwidXBkYXRlRGlhZ3JhbSI6ZmFsc2V9)

---