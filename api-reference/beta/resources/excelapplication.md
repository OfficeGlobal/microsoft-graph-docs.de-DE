---
title: Anwendung Ressourcentyp
description: Stellt die Excel-Anwendung dar, die die Arbeitsmappe verwaltet.
localization_priority: Normal
ms.openlocfilehash: a8e2124910301818e753b1f90a3168da3a072862
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804438"
---
# <a name="application-resource-type"></a>Anwendung Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
