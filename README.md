# Value breakdown

**This is a draft extension and is not recommended for use. Please contribute to [this GitHub issue](https://github.com/open-contracting/standard/issues/1070).**

Adds a value breakdown array to the Item, Award and Contract objects, to breakdown their total amounts.

## Example

```json
{
  "awards": [
    {
      "id": "25164528",
      "title": "ORDEN DE COMPRA DESDE 3489-12-LP14",
      "description": "Construcción Parque Comunal Thiers DESDE 3489-12-LP14",
      "status": "active",
      "date": "2020-08-27T11:40:47Z",
      "value": {
        "amount": 1128369415.0,
        "currency": "CLP"
      },
      "valueBreakdown": [
        {
          "id": "net",
          "description": "Precio total neto",
          "value": {
            "amount": 1128369415.0,
            "currency": "CLP"
          }
        },
        {
          "id": "charges",
          "description": "Cargos",
          "value": {
            "amount": 214390188.85,
            "currency": "CLP"
          }
        },
        {
          "id": "taxes",
          "description": "Impuestos",
          "value": {
            "amount": 214390188.85,
            "currency": "CLP"
          }
        }
      ]
    }
  ]
}
```
## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.

This extension was originally discussed in <https://github.com/open-contracting/standard/issues/1070>
