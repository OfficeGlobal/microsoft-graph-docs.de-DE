---
title: Ressourcentyp oneNoteIdentitySet
description: '**Unterstützung in Kürze verfügbar**'
localization_priority: Normal
ms.openlocfilehash: d2969d073503a9fd586641abeb3d82f719db8545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874088"
---
# <a name="onenoteidentityset-resource-type"></a>Ressourcentyp oneNoteIdentitySet

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

**Unterstützung in Kürze verfügbar**

Der OneNoteIdentitySet-Typ ist eine verschlüsselte Auflistung von [OneNoteIdentity](onenoteidentity.md) -Objekten.
Es wird verwendet, um einen Satz von Identitäten zugeordnet sind verschiedene Ereignisse für einen _Notizbuch_, einem _Bereich_ oder einer _Seite_, z. B. _von erstellt_ oder _zuletzt geändert von_darstellen. 
 
Aktuell enthält einen einzelnen Schlüssel, _**Benutzer**_.  In Zukunft können die Schlüssel wie das Gerät oder einer Anwendung das Element hinzugefügt werden.

In Zukunft werden sollen dieses Typs mit [IdentitySet](identityset.md) zusammengeführt

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|Eine OneNoteIdentity-Ressource, die einen Benutzer darstellt.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
