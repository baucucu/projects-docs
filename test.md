# Testing the Markdown copilot

**copilot** create table of contents

## Heading examples
### H1
## H2
### H3
#### H4
##### H5
###### H6


## Table example

<table>
    <style>
        table {
            width: 100%;
        }
    </style>
    <thead>
        <tr>
            <th>Layer 1</th>
            <th>Layer 2</th>
            <th>Layer 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=4>L1 Name</td>
            <td rowspan=2>L2 Name A</td>
            <td>L3 Name A</td>
        </tr>
        <tr>
            <td>L3 Name B</td>
        </tr>
        <tr>
            <td rowspan=2>L2 Name B</td>
            <td>L3 Name C</td>
        </tr>
        <tr>
            <td>L3 Name D</td>
        </tr>
        <tr>
            <td colspan=3>Merged</td>
        </tr>
        <tr>
            <td>L1 Second</td>
            <td>L2 Second</td>
            <td>L3 Second</td>
        </tr>
    </tbody>
</table>

## Mermaid JS gantt

```mermaid
gantt
    title Git Issues - days since last update
    dateFormat X
    axisFormat %s
    section Issue19062
    71   : 0, 71
    section Issue19401
    36   : 0, 36
    section Issue193
    34   : 0, 34
    section Issue7441
    9    : 0, 9
    section Issue1300
    5    : 0, 5
```

## Mermaid JS sequence diagram

```mermaid
sequenceDiagram
    Alice ->> Bob: Hello Bob, how are you?
    Bob-->>John: How about you John?
    Bob--x Alice: I am good thanks!
    Bob-x John: I am good thanks!
    Note right of John: Bob thinks a long<br/>long time, so long<br/>that the text does<br/>not fit on a row.

    Bob-->Alice: Checking with John...
    Alice->John: Yes... John, how are you?

```

## Mermaid JS flowchart

```mermaid
flowchart TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
```

## Mermaid JS user story

```mermaid
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```

## Mermaid JS class diagram

```mermaid
---
title: Animal example
---
classDiagram
    note "From Duck till Zebra"
    Animal <|-- Duck
    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"
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
        +bool is_wild
        +run()
    }

```

## Mermaid JS entity relationship diagram

```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    PRODUCT ||--|{ LINE-ITEM : includes
```

## Markdown features examples

### Unordered List examples

- Item 1
  - Item 2
- Item 3
  - Item 4
  - Item 5
    - Item 6

### Ordered List examples

1. Item 1
    1. Item 2
2. Item 3
    1. Item 4
    2. Item 5
        1. Item 6

### Code examples

#### JSON

```json
{
    "name": "John",
    "age": 30,
    "city": "New York",
    "hasChildren": false,
    "titles": [
        "engineer",
        "programmer",
        "designer"
    ],
    "address": {
        "street": "123 Main St",
        "city": "New York",
        "state": "NY",
    }
}
```

#### YAML

```yaml
name: John
age: 30
city: New York
hasChildren: false
titles:
  - engineer
  - programmer
  - designer
address:
  street: 123 Main St
  city: New York
  state: NY
```

#### JAVA BPMN

```java
public class MyProcess {
    public static void main(String[] args) {
        System.out.println("Hello World!");
        System.exit(0);
    }
}
```

### HTML examples

```html
<html>
    <body>
        <h1>Hello World</h1>
        <p>This is my first paragraph.</p>
    </body>
</html>
```

### Formatted text

```text
Hello World
This is my first paragraph.
```
