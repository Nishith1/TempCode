# TempCode

{
  "script": {
    "description": "Generic SpEL script to convert all attributes of an input object to string",
    "inputObject": {
      "name": "Alice",
      "age": 30,
      "salary": 75000.50,
      "id": 1234567890123456789,
      "bonus": 1500.75,
      "active": true,
      "createdAt": "2025-03-17T10:15:30"
    },
    "expressions": [
      {
        "attribute": "name",
        "expression": "T(String).valueOf('Alice')"
      },
      {
        "attribute": "age",
        "expression": "T(String).valueOf(30)"
      },
      {
        "attribute": "salary",
        "expression": "T(String).valueOf(75000.50)"
      },
      {
        "attribute": "id",
        "expression": "T(String).valueOf(1234567890123456789)"
      },
      {
        "attribute": "bonus",
        "expression": "T(String).valueOf(T(java.math.BigDecimal).valueOf(1500.75))"
      },
      {
        "attribute": "active",
        "expression": "T(String).valueOf(true)"
      },
      {
        "attribute": "createdAt",
        "expression": "T(String).valueOf('2025-03-17T10:15:30')"
      }
    ],
    "outputObject": {
      "name": "Alice",
      "age": "30",
      "salary": "75000.50",
      "id": "1234567890123456789",
      "bonus": "1500.75",
      "active": "true",
      "createdAt": "2025-03-17T10:15:30"
    }
  }
}
