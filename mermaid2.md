# Mermaid Diagram Examples

This file contains various Mermaid diagram examples for documentation and visualization purposes.

## Git Commit Timeline

```mermaid
gitgraph
    commit id: "c71cef8: fix: HM-174 connector template admin improvements"
    commit id: "231ad14: fix: HM-174 div to scrollarea"
    commit id: "d080f33: fix: HM-174 snakecasing to camelcasing"
    commit id: "ec1ed73: fix: HM-174 scroll event to intersection observer"
    commit id: "7632963: Merge branch 'develop' into feature/HM-1174-admin-connector-template-improvements"
```

## Alternative Git Timeline (Timeline View)

```mermaid
timeline
    title Git Commit History - HM-174 Feature Branch
    
    Oct 22, 2025 : fix: HM-174 connector template admin improvements
                 : Chidambaranathan S authored 5 days ago
                 : Commit: c71cef8
    
    Oct 24, 2025 : fix: HM-174 div to scrollarea
                 : Chidambaranathan S authored 3 days ago
                 : Commit: 231ad14
                 
                 : fix: HM-174 snakecasing to camelcasing
                 : Chidambaranathan S authored 3 days ago
                 : Commit: d080f33
                 
                 : fix: HM-174 scroll event to intersection observer
                 : Chidambaranathan S authored 3 days ago
                 : Commit: ec1ed73
    
    Oct 27, 2025 : Merge branch 'develop' into feature/HM-1174-admin-connector-template-improvements
                 : Chidambaranathan S authored 19 hours ago
                 : Commit: 7632963
```

## Flowchart Example

```mermaid
flowchart TD
    A[Start] --> B{Is it?}
    B -->|Yes| C[OK]
    C --> D[Rethink]
    D --> B
    B ---->|No| E[End]
```

## Sequence Diagram Example

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```

## Gantt Chart Example

```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    another task      : 24d
```

## Class Diagram Example

```mermaid
classDiagram
    class Animal {
        +String name
        +int age
        +makeSound()
    }
    class Dog {
        +String breed
        +bark()
    }
    class Cat {
        +String color
        +meow()
    }
    Animal <|-- Dog
    Animal <|-- Cat
```

## State Diagram Example

```mermaid
stateDiagram-v2
    [*] --> Still
    Still --> [*]
    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```