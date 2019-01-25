---
title: Anwendung Ressourcentyp
description: Stellt die Excel-Anwendung dar, die die Arbeitsmappe verwaltet.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 48ee13a67d97f9c5c1a96a6ef6e104c5629f4108
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517617"
---
# <a name="application-resource-type"></a>Anwendung Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Excel-Anwendung dar, die die Arbeitsmappe verwaltet.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen der Anwendung](../api/excelapplication-get.md) | [Anwendung](application.md) |Lesen Sie Eigenschaften und Beziehungen des Application-Objekts.|
|[Calculate](../api/excelapplication-calculate.md)|Keine|Alle in Excel geöffnete Arbeitsmappen werden neu berechnet.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|calculationMode|string|Gibt den Berechnungsmodus in der Arbeitsmappe verwendet. Mögliche Werte sind: `Automatic`, `AutomaticExceptTables` und `Manual`. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/excelapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
