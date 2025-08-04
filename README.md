# LoL
```mermaid
flowchart TD
    A([Start]) --> B([Display First Question])
    B --> C{Did the user input an answer?}
    C -->|Yes| D([Check Answer])
    C -->|No| E([Show Reminder: "Please answer before proceeding"])
    E --> B

    D --> F{Are there more questions?}
    F -->|Yes| G([Display Next Question])
    G --> H{Did the user input an answer?}
    H -->|Yes| I([Check Answer])
    H -->|No| J([Show Reminder: "Please answer before proceeding"])
    J --> G

    I --> F

    F -->|No| K([Display Score])
    K --> L([End])
```
