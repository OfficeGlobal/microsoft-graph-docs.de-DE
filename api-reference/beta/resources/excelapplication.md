---
title: Anwendung Ressourcentyp
description: Stellt die Excel-Anwendung dar, die die Arbeitsmappe verwaltet.
ms.openlocfilehash: 1772d69b55d03bf62d983a6dfb818dca651ebbd6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061371"
---
# <a name="application-resource-type"></a>Anwendung Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Excel-Anwendung dar, die die Arbeitsmappe verwaltet.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen der Anwendung](../api/excelapplication-get.md) | [Application](application.md) |Lesen Sie Eigenschaften und Beziehungen des Application-Objekts.|
|[Calculate](../api/excelapplication-calculate.md)|Keines|Alle in Excel geöffnete Arbeitsmappen werden neu berechnet.|

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
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->