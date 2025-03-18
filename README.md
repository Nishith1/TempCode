{
  "script": {
    "description": "Generic SpEL script to convert all attributes of an input object to string using variables",
    "inputObject": {
      "${name}": "${nameValue}",
      "${age}": "${ageValue}",
      "${salary}": "${salaryValue}",
      "${id}": "${idValue}",
      "${bonus}": "${bonusValue}",
      "${active}": "${activeValue}",
      "${createdAt}": "${createdAtValue}"
    },
    "typeCheckAndConversion": {
      "${name}": {
        "originalType": "T(${nameValue}.getClass()).getSimpleName()",
        "convertedType": "String",
        "value": "T(String).valueOf(${nameValue})"
      },
      "${age}": {
        "originalType": "T(${ageValue}.getClass()).getSimpleName()",
        "convertedType": "String",
        "value": "T(String).valueOf(${ageValue})"
      },
      "${salary}": {
        "originalType": "T(${salaryValue}.getClass()).getSimpleName()",
        "convertedType": "String",
        "value": "T(String).valueOf(${salaryValue})"
      },
      "${id}": {
        "originalType": "T(${idValue}.getClass()).getSimpleName()",
        "convertedType": "String",
        "value": "T(String).valueOf(${idValue})"
      },
      "${bonus}": {
        "originalType": "T(${bonusValue}.getClass()).getSimpleName()",
        "convertedType": "String",
        "value": "T(String).valueOf(${bonusValue})"
      },
      "${active}": {
        "originalType": "T(${activeValue}.getClass()).getSimpleName()",
        "convertedType": "String",
        "value": "T(String).valueOf(${activeValue})"
      },
      "${createdAt}": {
        "originalType": "T(${createdAtValue}.getClass()).getSimpleName()",
        "convertedType": "String",
        "value": "T(String).valueOf(${createdAtValue})"
      }
    },
    "outputObject": {
      "${name}": "T(String).valueOf(${nameValue})",
      "${age}": "T(String).valueOf(${ageValue})",
      "${salary}": "T(String).valueOf(${salaryValue})",
      "${id}": "T(String).valueOf(${idValue})",
      "${bonus}": "T(String).valueOf(${bonusValue})",
      "${active}": "T(String).valueOf(${activeValue})",
      "${createdAt}": "T(String).valueOf(${createdAtValue})"
    }
  }
}
