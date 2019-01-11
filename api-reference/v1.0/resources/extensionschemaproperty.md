---
title: extensionSchemaProperty-Ressourcentyp
description: Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer schemaExtension-Definition zu definieren.
localization_priority: Normal
ms.openlocfilehash: 384f60c323ca6c6fb23d2f4811a6d2cb918bf844
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880570"
---
# <a name="extensionschemaproperty-resource-type"></a>extensionSchemaProperty-Ressourcentyp

Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer [schemaExtension](schemaextension.md)-Definition zu definieren.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|String| Der Name der stark typisierten Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.|
|type|String| Der Typ der Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.  Zulässige Werte sind *Binary, Boolean, DateTime, Integer* oder *String*.  Weitere Einzelheiten finden Sie in der Tabelle unten.|

#### <a name="supported-property-data-types"></a>Unterstützte Datentypen für Eigenschaften 
Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:

| Eigenschaftentyp | Bemerkungen |
|-------------|------------|
| Binär | Maximal 256 Bytes. |
| Boolean | Nicht unterstützt für Kontakte, Nachrichten, Ereignisse und Beiträge. |
| DateTime | Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert. |
| Ganze Zahl | 32-Bit-Wert. Nicht unterstützt für Kontakte, Nachrichten, Ereignisse und Beiträge. |
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
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
