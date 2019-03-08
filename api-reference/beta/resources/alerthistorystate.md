---
title: alertHistoryState-Ressourcentyp
description: Speichert an Warnungen vorgenommene Änderungen.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a7975d870389be5163a8f230f6a6cc4cd1425c3
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480831"
---
# <a name="alerthistorystate-resource-type"></a>alertHistoryState-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Speichert an Warnungen vorgenommene Änderungen.

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|appId|Zeichenfolge| Die Anwendungs-ID der aufrufenden Anwendung, die ein Update (PATCH) an die Warnung übermittelt hat. Die Anwendungs-ID sollte aus dem auth-Token extrahiert und nicht manuell von der aufrufenden Anwendung eingegeben werden. |
|assignedTo|Zeichenfolge| UPN des Benutzers, dem die Warnung zugewiesen wurde (Hinweis: Alert. ZugewiesenAn speichert nur den letzten Wert/UPN). |
|Kommentare|String collection|Vom angemeldeten Benutzer eingegebene Kommentar.|
|Feedback|Zeichenfolge| Analysten Feedback zu der Warnung in diesem Update. Mögliche Werte sind: `unknown`, `truePositive`, `falsePositive` und `benignPositive`.|
|status|String| Warnungsstatus Wert (falls aktualisiert). Mögliche Werte: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.|
|updatedDateTime|DateTimeOffset| Datum und Uhrzeit des Warnungs Updates. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|user|Zeichenfolge| UPN des angemeldeten Benutzers, der die Warnung aktualisiert hat (entnommen vom Bearer-Token, falls im Benutzer/Delegierten Authentifizierungsmodus). |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->