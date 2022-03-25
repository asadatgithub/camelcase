# Covert Dictionary to camelCase

This module is specifically designed to convert all snake_case attributes to camelCase.


In some cases, we need to follow both conventions. Like the python follows snake_case convention, on the other hand json uses camcelCase.

This module uses the basic python program to let us do that easly.

To convert a string to camel case

```
import camelcase
camelcase.to_camel_case("hello_world")
```
Result
```
helloWorld
```

Same goes for the dictionary
```
dictionary =  {
        "id": "string",
        "field_type": "numberfield",
        "field_label": "string",
        "field_id": "string",
        "read_only": True,
        "label_column": 0,
        "field_column": 0,
        "hidden": True,
        "required": True,
        "notes": "string",

        "help_text": "string",
        "validation": {
            "unique": True,
            "size": {
                "min": 0,
                "max": 0,
                "custom_message": "string"
            }
        },
        "data_type": 0,
        "regexp": {
            "pattern": "string",
            "flags": "string",
            "custom_message": "string"
        },
        "prohibit_pattern": {
            "pattern": "string",
            "flags": "string",
            "custom_message": "string"
        },
        "on_blur": "string",
        "on_change": "string",
        "placeholder": "string"
    }
    
camelcase.comel_case_dict(dictionary)

```

Result:
```
{
   "id":"string",
   "fieldType":"numberfield",
   "fieldLabel":"string",
   "fieldId":"string",
   "readOnly":true,
   "labelColumn":0,
   "fieldColumn":0,
   "hidden":true,
   "required":true,
   "notes":"string",
   "helpText":"string",
   "validation":{
      "unique":true,
      "size":{
         "min":0,
         "max":0,
         "customMessage":"string"
      }
   },
   "dataType":0,
   "regexp":{
      "pattern":"string",
      "flags":"string",
      "customMessage":"string"
   },
   "prohibitPattern":{
      "pattern":"string",
      "flags":"string",
      "customMessage":"string"
   },
   "onBlur":"string",
   "onChange":"string",
   "placeholder":"string"
}
```