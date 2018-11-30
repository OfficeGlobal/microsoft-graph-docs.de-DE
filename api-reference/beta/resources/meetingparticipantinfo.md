---
title: Ressourcentyp meetingParticipantInfo
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 1d9c22924f8f05255b5e01bad4bbcd6ae5957ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061808"
---
# <a name="meetingparticipantinfo-resource-type"></a>Ressourcentyp meetingParticipantInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ                          | Beschreibung                              |
|:---------------|:------------------------------|:-----------------------------------------|
| Identität       | [identitySet](identityset.md) | Identitätsinformationen des Teilnehmers. |
| UPN            | String                        | Benutzerprinzipalname des Teilnehmers.  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
