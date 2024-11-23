# Simple gantt

``` mermaid
gantt
    title A Gantt Diagram

    Completed task            :done,    task, 2024-01-06,2024-01-08
    Active task               :active,  task2, 2024-01-09, 3d
    Future task               :         task3, after task2, 5d
    Future task2              :         task4, after task3, 5d
```