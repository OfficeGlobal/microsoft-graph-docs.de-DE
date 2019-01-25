---
title: Ressourcentyp onPremisesPublishing
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508181"
---
# <a name="onpremisespublishing-resource-type"></a>Ressourcentyp onPremisesPublishing

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|customDomainCertificate|String|Details des Zertifikats mit der Anwendung verbunden sind, wenn eine benutzerdefinierte Domäne verwendet wird. NULL, wenn die Standarddomäne zu verwenden.|
|externalAuthenticationType|String|Details der Vorauthentifizierung-Einstellung für die Anwendung möglichen Werte sind: `passthru`, `aadPreAuthentication`.|
|externalUrl|String|Die veröffentlichte externe Url für die Anwendung. Beispiel: https://intranet-contoso.msappproxy.net/  |
|internalUrl|String|Die interne Url der Anwendung. Beispiel: https://intranet/ |
|isOnPremPublishingEnabled|Boolescher Wert|Gibt an, ob die Anwendung derzeit oder nicht veröffentlicht wird.|
|applicationServerTimeout|String|Die Dauer der Verbindung eine Antwort aus der Back-End-Anwendung vor dem Schließen der Verbindungs wartet. Mögliche Werte sind: `default` und `long`. Verwendung `long` Wenn Ihr Server mehr als 60 75 Sekunden reagiert auf Anforderungen dauert. Versuchen Sie außerdem `long` Wenn Sie nicht sind auf die Anwendung zugreifen und der Fehlerstatus "Backend Timeout" ist.|
|isTranslateHostHeaderEnabled|Boolescher Wert|Gibt an, ob die Anwendung Urls in der Antwort-Headern übersetzen sollten. Dies beinhaltet das Festlegen der richtigen Website für Cookies.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
