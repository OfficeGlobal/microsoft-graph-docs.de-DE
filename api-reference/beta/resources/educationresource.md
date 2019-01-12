---
title: Ressourcentyp educationResource
description: Eine übergeordnete Klasse für alle Resource-Objekten im System. Eine Ressource ist eine **Zuordnung** und/oder **Übermittlung**, das das Learning-Objekt darstellt, das wird zugeordnet
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ac84fd9d661f31186ea65e95c680456cdabe221
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982120"
---
# <a name="educationresource-resource-type"></a>Ressourcentyp educationResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine übergeordnete Klasse für alle Resource-Objekten im System. Eine Ressource ist zugeordnet, mit einer **Zuordnung** und/oder **Übermittlung**, das das Learning-Objekt darstellt, das wird ausgegeben werden, oder übergeben. Eine Ressource kann nicht direkt instanziiert werden. Sie müssen eine Unterklasse vornehmen, die den Typ der Ressource verwendeten darstellt.

Diese Ressource werden die allgemeinen Eigenschaften für alle Arten von Ressource gespeichert.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Die die Ressource erstellt.|
|createdDateTime|-Zeitpunkt der Erstellung die Ressource.  DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|displayName|Zeichenfolge|Der Anzeigename der Ressource.|
|lastModifiedBy|[identitySet](identityset.md)|Wer war der letzte Benutzer, die Ressource zu ändern.|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt der Uhrzeit der letzten die Ressource Änderung.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
