---
title: Ressourcentyp signInStatus
description: Stellt die Anmeldestatus (Erfolg oder Fehler) von der Anmeldung
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878638"
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
