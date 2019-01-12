---
title: WorksheetProtection-Ressourcentyp
description: Stellt den Schutz eines Arbeitsblattobjekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5b9faed56e545698cb731728b2c95fd31682b252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916992"
---
# <a name="worksheetprotection-resource-type"></a>WorksheetProtection-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt den Schutz eines Arbeitsblattobjekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get WorksheetProtection](../api/worksheetprotection-get.md) | [WorksheetProtection](worksheetprotection.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des worksheetProtection-Objekts.|
|[Protect](../api/worksheetprotection-protect.md)|Keine|Schützen ein Arbeitsblatt. Wird ausgelöst, wenn das Arbeitsblatt geschützt ist.|
|[Unprotect](../api/worksheetprotection-unprotect.md)|Keine|Schutz eines Arbeitsblatts aufheben.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|geschützt|boolean|Zeigt an, ob das Arbeitsblatt geschützt ist.  Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|options|[WorksheetProtectionOptions](worksheetprotectionoptions.md)|Optionen für den Arbeitsblattschutz. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
