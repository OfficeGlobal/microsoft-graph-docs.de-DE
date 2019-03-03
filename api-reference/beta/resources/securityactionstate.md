---
title: securityActionState-Ressourcentyp
description: Stellt den Verlauf der Änderungen des SecurityAction-Zustands dar.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8f789dab438316f16b9c2607947fa08b7fcefdc2
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366931"
---
# <a name="securityactionstate-resource-type"></a>securityActionState-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Verlauf der Änderungen des SecurityAction-Zustands dar.

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|appId|Zeichenfolge|Die Anwendungs-ID der aufrufenden Anwendung, die ein Update (PATCH) an die Aktion gesendet hat. Der `appId` sollte aus dem auth-Token extrahiert und nicht manuell von der aufrufenden Anwendung eingegeben werden.|
|status|Zeichenfolge| Status der SecurityAction in diesem Update. Mögliche Werte: `NotStarted`, `Running`, `Completed`, `Failed`.|
|updatedDateTime|DateTimeOffset| Timestamp, als der Actionstate wurden aktualisiert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|user|Zeichenfolge|Der Benutzerprinzipalname des angemeldeten Benutzers, der ein Update (PATCH) an die Aktion gesendet hat. Der `user` sollte aus dem auth-Token extrahiert und nicht manuell von der aufrufenden Anwendung eingegeben werden.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
