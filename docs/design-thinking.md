graph LR
    A[开始<br/>] --> B[需求解析]
    B --> C[代码执行]
    C --> D{条件分支<br/>IF 代码执行result是True OR 代码执行result不是False<br/>ELSE}
    D -->|True| E[知识检索]
    D -->|False| F[信息追问]
    E --> G[策略生成]
    F --> H[回复信息追问结果]
    G --> I[回复策略生成结果]
    
