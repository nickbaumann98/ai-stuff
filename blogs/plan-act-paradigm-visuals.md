# Visual Diagrams for Plan-Act Paradigm Blog

## 1. The Evolution of AI Coding - Effort Distribution

```mermaid
pie title "Tab Autocomplete Era"
    "Human Effort (Navigation, Planning, Typing, Debugging)" : 95
    "AI Effort (Suggestions)" : 5
```

```mermaid
pie title "Agentic AI Era"
    "AI Effort (Searching, Reading, Writing, Refactoring)" : 95
    "Human Effort (Intent)" : 5
```

## 2. The Plan-Act Paradigm Flow (Not Modes, But Phases)

```mermaid
graph LR
    A[Human Intent] -->|Plan Phase| B[Intent Gathering]
    B --> C[Mutual Understanding]
    C -->|Act Phase| D[Get Out of the Way]
    D --> E[Uninterrupted Execution]
    E --> F[Human Evaluation]
    F -->|If needed| A
    
    style A fill:#ff9999
    style B fill:#99ccff
    style C fill:#99ccff
    style D fill:#99ff99
    style E fill:#99ff99
    style F fill:#ff9999
```

## 3. Interrupted Context vs Fresh Start

```mermaid
graph TD
    subgraph "Interrupted Context"
        I1[Initial Task] --> I2[Partial Progress]
        I2 --> I3[❌ Interruption]
        I3 --> I4[Context Confusion]
        I4 --> I5[Degraded Performance]
    end
    
    subgraph "Fresh Start"
        F1[Clear Intent] --> F2[Clean Narrative]
        F2 --> F3[Coherent Execution]
        F3 --> F4[Better Results]
    end
    
    style I3 fill:#ff6666
    style I4 fill:#ff9999
    style I5 fill:#ffcccc
    style F1 fill:#66ff66
    style F2 fill:#99ff99
    style F3 fill:#99ff99
    style F4 fill:#ccffcc
```

## 4. The Anti-Persona Philosophy

```mermaid
graph TD
    subgraph "Traditional Approach"
        T1[Base Model] --> T2[Debugger Agent]
        T1 --> T3[Architect Agent]
        T1 --> T4[Code Reviewer Agent]
        T2 --> T5[Limited Scope]
        T3 --> T5
        T4 --> T5
    end
    
    subgraph "Cline's Approach"
        C1[Full Model Capabilities] --> C2[All Skills Available]
        C2 --> C3[Better Performance]
    end
    
    style T5 fill:#ffcccc
    style C3 fill:#ccffcc
```

## 5. The Slot Machine Principle - Parallel Futures

```mermaid
graph LR
    A[Clear Intent] --> B1[Attempt 1]
    A --> B2[Attempt 2]
    A --> B3[Attempt 3]
    
    B1 --> C1[Result A]
    B2 --> C2[Result B]
    B3 --> C3[Result C]
    
    C1 --> D[Choose Best]
    C2 --> D
    C3 --> D
    
    style A fill:#99ccff
    style D fill:#99ff99
```

## 6. Safety Through Timing

```mermaid
timeline
    title The Right Time for Control
    
    Plan Phase : Gather Requirements
               : Share Intent
               : Set Boundaries
               : Define Constraints
    
    Act Phase  : Let AI Execute
               : No Interruptions
               : Full Auto-Approve
               : Maintain Flow
    
    Review     : Evaluate Results
               : Use Checkpoints
               : Undo if Needed
               : Iterate
```

## 7. Evolution of Intent Sharing

```mermaid
graph TB
    A[Today: Text-Based Intent] --> B[Near Future: Voice Interfaces]
    B --> C[Visual Sketching Tools]
    C --> D[Collaborative Sessions]
    D --> E[Direct Neural Interfaces?]
    
    style A fill:#cccccc
    style B fill:#add8e6
    style C fill:#87ceeb
    style D fill:#4682b4
    style E fill:#191970,color:#fff
```

## 8. The Human-AI Collaboration Loop

```mermaid
stateDiagram-v2
    [*] --> HumanIntent: Task Begins
    HumanIntent --> PlanPhase: Share Requirements
    PlanPhase --> MutualUnderstanding: AI Asks Questions
    MutualUnderstanding --> ActPhase: Clear Intent Achieved
    ActPhase --> AIExecution: Autonomous Work
    AIExecution --> Results: Task Complete
    Results --> HumanReview: Evaluate
    HumanReview --> [*]: Accept
    HumanReview --> HumanIntent: Refine & Retry
    
    note right of PlanPhase: Same AI, optimized for intent gathering
    note right of ActPhase: Same AI, optimized for execution
    note right of HumanReview: Checkpoints enable safety
```

---

These diagrams can be embedded directly in the blog post or used in presentations about the Plan-Act paradigm. Each visual reinforces a key concept from the written content.
