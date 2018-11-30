---
title: Ressourcentyp signInStatus
description: Stellt die Anmeldestatus (Erfolg oder Fehler) von der Anmeldung
ms.openlocfilehash: cafa0dffe1b1d798d87225ac82901cf041d5e4fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064987"
---
# <a name="signinstatus-resource-type"></a>Ressourcentyp signInStatus
Stellt die Anmeldestatus (Erfolg oder Fehler) von der Anmeldung



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|additionalDetails|String|Bietet zusätzliche Details für die Aktivität-Anmeldung|
|errorCode|Int32|Enthält den 5 6digit Fehlercode, der bei einem Ausfall-Anmeldung generiert wird. Checken Sie die [Liste der Fehlercodes und Nachrichten](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|String|Enthält die Fehlermeldung oder der Fehlerursache für die entsprechende Aktivität-Anmeldung. Checken Sie die [Liste der Fehlercodes und Nachrichten](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->