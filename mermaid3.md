# Mermaid Diagram Examples - HM-1174 Project

This document contains Mermaid diagrams documenting the HM-1174 project timeline and structure.

## Git Graph Example - HM-1174 Project Timeline

```mermaid
gitgraph
    commit id: "Initial commit"
    commit id: "Base setup"
    branch feature/HM-1174-admin-connector-template-improvements
    checkout feature/HM-1174-admin-connector-template-improvements
    commit id: "c71cef8: connector template admin improvements"
    commit id: "231ad14: div to scrollarea"
    commit id: "d080f33: snakecasing to camelcasing"
    commit id: "ec1ed73: scroll event to intersection observer"
    checkout main
    merge feature/HM-1174-admin-connector-template-improvements
    commit id: "7632963: Merge develop branch"
```

## Project Timeline

- **Oct 27, 2025**: Merge branch 'develop' into feature/HM-1174-admin-connector-template-improvements
  - Author: Chidambaranathan S
  - Time: 19 hours ago
  - Commit: `7632963`

- **Oct 24, 2025**: Multiple fixes implemented
  - fix: HM-1174 scroll event to intersection observer (3 days ago) - `ec1ed73`
  - fix: HM-1174 snakecasing to camelcasing (3 days ago) - `d080f33`
  - fix: HM-1174 div to scrollarea (3 days ago) - `231ad14`

- **Oct 22, 2025**: Initial feature implementation
  - fix: HM-1174 connector template admin improvements (5 days ago) - `c71cef8`

## Flowchart - Feature Development Process

```mermaid
flowchart TD
    A[Start: HM-1174 Task] --> B[Create Feature Branch]
    B --> C[Implement connector template admin improvements]
    C --> D[Fix: div to scrollarea]
    D --> E[Fix: snakecasing to camelcasing]
    E --> F[Fix: scroll event to intersection observer]
    F --> G{Code Review}
    G -->|Approved| H[Merge to develop]
    G -->|Changes needed| C
    H --> I[Merge develop to feature branch]
    I --> J[Deploy]
```

## Sequence Diagram - Development Workflow

```mermaid
sequenceDiagram
    participant Dev as Developer
    participant FB as Feature Branch
    participant DB as Develop Branch
    participant MB as Main Branch
    
    Dev->>FB: Create feature/HM-1174-admin-connector-template-improvements
    Dev->>FB: Commit c71cef8: connector template improvements
    Dev->>FB: Commit 231ad14: div to scrollarea
    Dev->>FB: Commit d080f33: snakecasing to camelcasing
    Dev->>FB: Commit ec1ed73: scroll event to intersection observer
    FB->>DB: Merge feature changes
    DB->>FB: Merge back (7632963)
    FB->>MB: Ready for production
```