# Empresa Fake 2025 - Cenário do Funcionário 
Java RESTful criada para a Empresa Fake.

## Diagrama de classes

```mermaid
classDiagram
    class Client {
        +int id
        +String name
    }

    class Product {
        +int id
        +String name
    }

    class Region {
        +int id
        +String country
        +String state
        +String city
    }

    class Time {
        +int id
        +int year
        +int semester
        +int quarter
        +int month
        +int day
    }

    class Sale {
        +int id
        +int quantity
        +float totalValue
    }

    Client "1" --* "0..N" Sale : 
    Product "1" --* "1..N" Sale : 
    Region "1" --* "1..N" Sale : 
    Time "1" --* "1..N" Sale : 
 

```
