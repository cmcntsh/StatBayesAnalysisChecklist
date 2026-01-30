# StatBayesAnalysisChecklist

* Before modeling statistics, you need to think of a scientific causal model first. How are the phenomena of interest related to each other? Which variables "listen" other which others? Draw diagram with arrows.

Height influences weight. Sex influences both height and weight. Weight is influenced by both height and sex.

```mermaid
graph LR
   H-->W
   S-->H
   S-->W

```

```mermaid
graph TD
    subgraph top [ ]
        direction LR
        H --- W
    end
    S --> H
    S --> W
    H --> W
    
    %% Styling to hide the subgraph container
    style top fill:none,stroke:none
```
