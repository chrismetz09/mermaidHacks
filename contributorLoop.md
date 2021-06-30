
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