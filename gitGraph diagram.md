## Simple gitGraph diagram

``` mermaid
gitGraph:
    commit id: "Initial commit"
    commit id: "Did stuff"
    
    branch branchingOff
    
    checkout branchingOff
    commit id: "Did some branch stuff"
    commit id: "Did more branch stuff"
    checkout main
    commit id: "Did some more stuff"
    merge branchingOff id: "Merging back"

    commit id: "Post merge stuff"
    commit id: "Final?"
```