---
title: extensionSchemaProperty-Ressourcentyp
description: Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer schemaExtension-Definition zu definieren.
ms.openlocfilehash: f699ccebefc849a7bf9cacc6dbda61cbcbb9896d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059760"
---
# <a name="extensionschemaproperty-resource-type"></a>extensionSchemaProperty-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer [schemaExtension](schemaextension.md)-Definition zu definieren.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|String| Der Name der stark typisierten-Eigenschaft als Teil einer schemaerweiterung definiert.|
|Typ|String| Der Typ der Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.  Zulässige Werte sind *Binary, Boolean, DateTime, Integer* oder *String*.  Weitere Einzelheiten finden Sie in der Tabelle unten.|

#### <a name="supported-property-data-types"></a>Unterstützte Datentypen für Eigenschaften 
Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:

| Eigenschaftentyp | Bemerkungen |
|-------------|------------|
| Binär | Maximal 256 Bytes. |
| Boolescher Wert | Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| DateTime | Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert. |
| Ganze Zahl | 32-Bit-Wert. Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| String | Maximal 256 Zeichen. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->