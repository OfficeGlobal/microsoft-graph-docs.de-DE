---
title: Ressourcentyp meetingParticipantInfo
description: Informationen über einen Teilnehmer an einer Besprechung.
author: VinodRavichandran
ms.openlocfilehash: 2bbb410ea26640ec05d66b5beb0c4b4ea24a42bd
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380198"
---
# <a name="meetingparticipantinfo-resource-type"></a>Ressourcentyp meetingParticipantInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Informationen über einen Teilnehmer an einer Besprechung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ                          | Beschreibung                              |
|:---------------|:------------------------------|:-----------------------------------------|
| Identität       | [identitySet](identityset.md) | Identitätsinformationen des Teilnehmers. |
| UPN            | Zeichenfolge                        | Benutzerprinzipalname des Teilnehmers.  |

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
