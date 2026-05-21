 A["用户输入"] --> B["需求解析"]
    B --> C["信息完整性判断"]
    C --> D{"条件分支"}
    D -- 信息不足 --> E["追问"]
    E --> A
    D -- 信息充分 --> F["生成结果"]
    F --> n1["直接回复"]

     A:::inputNode
     B:::processNode
     C:::processNode
     D:::decisionNode
     E:::feedbackNode
     F:::outputNode
     n1:::inputNode
    classDef decisionNode stroke:#fb923c,fill:#fff7ed
    classDef outputNode stroke:#4ade80,fill:#f0fdf4
    classDef feedbackNode stroke:#f87171,fill:#fef2f2
    classDef processNode stroke:#2dd4bf, fill:#f0fdfa
    classDef inputNode stroke:#818cf8, fill:#eef2ff
    style n1 color:#424242
    
