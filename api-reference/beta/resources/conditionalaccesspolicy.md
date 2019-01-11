---
title: Ressourcentyp conditionalAccessPolicy
description: Gibt an, dass die Attribute, die weiterführende eine bedingte Zugriffsrichtlinie oder Richtlinien, die von der entsprechenden Anmeldung Aktivität ausgelöst wird
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820643"
---
# <a name="conditionalaccesspolicy-resource-type"></a>Ressourcentyp conditionalAccessPolicy
Gibt an, dass die Attribute, die weiterführende eine bedingte Zugriffsrichtlinie oder Richtlinien, die von der entsprechenden Anmeldung Aktivität ausgelöst wird



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|String|Verweist auf den Namen der Richtlinie bedingten Zugriff (Beispiel: "Mehrstufiger Authentifizierung das für Vertriebs erfordern").|
|enforcedGrantControls|Collection von Objekten des Typs „String“|Bezieht sich auf die Grant-Steuerelemente, die durch die bedingte Zugriffsrichtlinie erzwungen (Beispiel: "Erfordern Multi-Factor Authentication").|
|enforcedSessionControls|Collection von Objekten des Typs „String“|Bezieht sich auf die Sitzung-Steuerelemente, die durch die bedingte Zugriffsrichtlinie erzwungen (Beispiel: "Erfordern app erzwungen Steuerelemente").|
|id|String|Eindeutige GUID bedingte-Richtlinie|
|result|String| Gibt das Ergebnis der Zertifizierungsstellenrichtlinie, die ausgelöst wurde. Mögliche Werte sind:<br/> `success` <br/> `failure` <br/> `notApplied`-Richtlinie wird nicht angewendet, da Drahtloszugriff nicht erfüllt wurden. <br/> `notEnabled`-Dies ist aufgrund der Richtlinie in deaktiviertem Zustand.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
