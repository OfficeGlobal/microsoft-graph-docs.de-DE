---
title: extensionSchemaProperty-Ressourcentyp
description: Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer schemaExtension-Definition zu definieren.
localization_priority: Normal
ms.openlocfilehash: bb044aa2f85ea5accdba4ed43a1a5b1c856a209d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511506"
---
# <a name="extensionschemaproperty-resource-type"></a>extensionSchemaProperty-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer [schemaExtension](schemaextension.md)-Definition zu definieren.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|Zeichenfolge| Der Name der stark typisierten-Eigenschaft als Teil einer schemaerweiterung definiert.|
|type|String| Der Typ der Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.  Zulässige Werte sind *Binary, Boolean, DateTime, Integer* oder *String*.  Weitere Einzelheiten finden Sie in der Tabelle unten.|

#### <a name="supported-property-data-types"></a>Unterstützte Datentypen für Eigenschaften 
Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:

| Eigenschaftentyp | Bemerkungen |
|-------------|------------|
| Binär | Maximal 256 Bytes. |
| Boolescher Wert | Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| DateTime | Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert. |
| Ganze Zahl | 32-Bit-Wert. Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| Zeichenfolge | Maximal 256 Zeichen. |

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
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/extensionschemaproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
