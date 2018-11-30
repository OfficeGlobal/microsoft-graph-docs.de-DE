---
title: Ressourcentyp privilegedRoleSummary
description: Die Statistiken für eine bestimmte Rolle Zusammenfassung.
ms.openlocfilehash: f6c66433651eff188ce6fdaa07c2422d3bb6e0ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064652"
---
# <a name="privilegedrolesummary-resource-type"></a>Ressourcentyp privilegedRoleSummary

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Statistiken für eine bestimmte Rolle Zusammenfassung.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](privilegedrolesummary.md) |Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleSummary-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|elevatedCount|int32|Die Anzahl der Benutzer, die die Rolle zugewiesen haben, ist aktiviert.|
|id|string| Der eindeutige Bezeichner für die Rolle. Schreibgeschützt.|
|managedCount|int32|Die Anzahl der Benutzer, die die Rolle zugewiesen haben, aber die Rolle ist deaktiviert.|
|mfaEnabled|Boolean|**true,** Wenn die Rolle Aktivierung mehrstufiger Authentifizierung das erforderlich sind. **false,** Wenn die Rolle Aktivierung mehrstufiger Authentifizierung das erforderlich ist.|
|status|string| Mögliche Werte sind: `ok` und `bad`. Der Wert hängt das Verhältnis von (ManagedCount / UsersCount). Wenn das Verhältnis einen vordefinierten Schwellenwert unterschreitet `ok` wird zurückgegeben. Andernfalls `bad` wird zurückgegeben.|
|usersCount|int32|Die Anzahl der Benutzer, die mit der Rolle zugewiesen sind.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->