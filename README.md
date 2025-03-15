# User Class Diagram

```mermaid
classDiagram
    class User {
        +String name
    }
    
    class Account {
        +String agency
        +String number
        +float balance
        +float limit
    }
    
    class Feature {
        +String icon
        +String description
    }
    
    class Card {
        +String number
        +float limit
    }
    
    class News {
        +String icon
        +String description
    }
    
    User --> Account : has
    User --> "*" Feature : has
    User --> Card : has
    User --> "*" News : has
