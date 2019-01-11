---
title: Ressourcentyp onPremisesPublishing
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 30ff6908a42a690e07d71b5d0c62fcb22dea3c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842539"
---
# <a name="onpremisespublishing-resource-type"></a>Ressourcentyp onPremisesPublishing

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|customDomainCertificate|Zeichenfolge|Details des Zertifikats mit der Anwendung verbunden sind, wenn eine benutzerdefinierte Domäne verwendet wird. NULL, wenn die Standarddomäne zu verwenden.|
|externalAuthenticationType|Zeichenfolge|Details der Vorauthentifizierung-Einstellung für die Anwendung möglichen Werte sind: `passthru`, `aadPreAuthentication`.|
|externalUrl|Zeichenfolge|Die veröffentlichte externe Url für die Anwendung. Zum Beispielhttps://intranet-contoso.msappproxy.net/  |
|internalUrl|Zeichenfolge|Die interne Url der Anwendung. Zum Beispielhttps://intranet/ |
|isOnPremPublishingEnabled|Boolescher Wert|Gibt an, ob die Anwendung derzeit oder nicht veröffentlicht wird.|
|applicationServerTimeout|Zeichenfolge|Die Dauer der Verbindung eine Antwort aus der Back-End-Anwendung vor dem Schließen der Verbindungs wartet. Mögliche Werte sind `default`, `long`. Verwendung `long` Wenn Ihr Server mehr als 60 75 Sekunden reagiert auf Anforderungen dauert. Versuchen Sie außerdem `long` Wenn Sie nicht sind auf die Anwendung zugreifen und der Fehlerstatus "Backend Timeout" ist.|
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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
