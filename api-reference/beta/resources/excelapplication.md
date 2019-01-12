---
title: Anwendung Ressourcentyp
description: Stellt die Excel-Anwendung dar, die die Arbeitsmappe verwaltet.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 250141ff6c6da3a81a1b3492908bc2e04b5a0605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921976"
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
