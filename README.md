## Table of Contents
- [Code](#code)
- [Tables](#tables)
- [Call Outs](#call-outs)
- [Miscellaneous](#miscellaneous)
- [Charts](#charts)

# Level 1 Heading
## Level 2 Heading
### Level 3 Heading

## Code

Use `code` for inline text.

```json
{
    "software": {
        "name": "Name",
        "version": "1.0",
        "features": ["Feature 1", "Feature 2"]
    }
}
```

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

```javascript
function greet(name) {
    return `Hello, ${name}!`;
}
```

## Tables

| *Left-Aligned* | Center-Aligned | Right-Aligned |
|:---------------|:--------------:|--------------:|
| Item 1         |     Item 2     |       Item 3  |
| Item 4         |     Item 5     |       Item 6  |

|                | Header 1   | Header 2   |
| -------------- | ---------- | ---------- |
| **Subheader 1**| Content    | Content    |
| **Subheader 2**| Content    | Content    |


<table>
  <tr>
    <th>Header 1</th>
    <th colspan="2">Header 2</th>
  </tr>
  <tr>
    <td>Content 1</td>
    <td>Content 2</td>
    <td>Content 3</td>
  </tr>
</table>

## Call Outs

> [!NOTE]
> Remember to always save your progress before closing the application.

> [!TIP]
> Use keyboard shortcuts to boost your productivity while working.

> [!IMPORTANT]
> Make sure to regularly back up your data to avoid loss.

> [!WARNING]
> Avoid turning off your computer during updates to prevent system corruption.

> [!CAUTION]
> Be cautious when sharing personal information online; protect your privacy.

## Miscellaneous

### Links

- [Documents](https://documents.example.com)

### Collapsible Sections

<details>
  <summary>Click to expand</summary>
  <p>This content is hidden until you click the summary.</p>
</details>

<details>
  <summary>List of Items</summary>
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>
</details>

### Tasks

- [ ] Incomplete item
    - [x] Completed subitem
    - [ ] Incomplete subitem


### Keyboards Inputs

Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.

---

## Charts

### Flowchart

```mermaid
flowchart LR
    A --> B --> C
```

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

```mermaid
graph TD
    A[Start] --> B{Is it sunny?}
    B -- Yes --> C[Go for a walk]
    B -- No --> D[Read a book]
    C --> E[End]
    D --> E[End]
```

### Sequence Diagram

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>Bob: Hello Bob, how are you?
    Bob-->>Alice: I am good, thanks!
```

### Pie Chart

```mermaid
pie
    title Key Metrics
    "Sales" : 50
    "Marketing" : 30
    "Development" : 20
```

### Entity-Relationship Diagram (ERD)

```mermaid
erDiagram
    CUSTOMER {
        int id
        string name
    }
    ORDER {
        int id
        string date
        int customerId
    }
    PRODUCT {
        int id
        string name
        double price
    }
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ PRODUCT : contains
```

### Class Diagram

```mermaid
classDiagram
    Animal <|-- Duck
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool isWild
        +run()
    }
```

### State Diagram

```mermaid
stateDiagram
    [*] --> S1
    S1 --> S2
    S2 --> S3
    S3 --> [*]
```

```mermaid
stateDiagram
    [*] --> Init
    Init --> Running
    state Running {
        [*] --> Idle
        Idle --> Active
        Active --> Idle
    }
    Running --> Stopped
    Stopped --> [*]
```

### Gantt Chart

```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
        A task           :a1, 2022-01-01, 30d
        Another task     :after a1, 20d
    section Another
        Task in sec      :2022-02-01, 12d
        Another task     : 24d
```

### Mind Map

```mermaid
mindmap
  root((Root))
    First_Level_A
      Second_Level_A1
      Second_Level_A2
    First_Level_B
      Second_Level_B1
      Second_Level_B2
        Third_Level_B2a
        Third_Level_B2b
```
### User Journey Diagram

```mermaid
journey
    title User Journey
    section Browsing
      User opens homepage: 5: User
      User searches for products: 3: User
    section Checkout
      User adds product to cart: 5: User
      User proceeds to checkout: 2: User
      User completes payment: 4: User
```