flowchart TD
    A[Developers] --> B[GitLab Repository<br/>(Salesforce & AWS)]
    B --> C[GitLab CI/CD]

    C --> D[Salesforce Pipeline]
    C --> E[AWS Pipeline]

    D --> F[Tests, Build, Package,<br/>Scratch Orgs, Delta Deployment]
    E --> G[IaC, Build, Test,<br/>Terraform/CDK, Blue/Green]

    F --> H[Deployment to Salesforce]
    G --> I[Deployment to AWS]

    H --> J[Feedback & Status Reports]
    I --> J

    J --> K[Slack/MS Teams, Jira/Asana]
    K --> L[Continuous Monitoring & Optimization]

    style A fill:#0066CC,stroke:#004080,color:#fff
    style B fill:#0099FF,stroke:#0066CC,color:#fff
    style C fill:#00CC99,stroke:#007A66,color:#fff
    style D fill:#FF6600,stroke:#CC5200,color:#fff
    style E fill:#FF9900,stroke:#CC6600,color:#fff
    style F fill:#FF9966,stroke:#CC6600,color:#fff
    style G fill:#FFCC66,stroke:#CC9900,color:#000
    style H fill:#FF6600,stroke:#CC5200,color:#fff
    style I fill:#FF9900,stroke:#CC6600,color:#fff
    style J fill:#33CC99,stroke:#007A66,color:#fff
    style K fill:#3366CC,stroke:#003366,color:#fff
    style L fill:#660099,stroke:#33004D,color:#fff
