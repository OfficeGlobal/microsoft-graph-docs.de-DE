---
title: Ressourcentyp mfaDetail
description: 'Gibt Details für eine bestimmte Anmeldung mehrstufiger Authentifizierung das an. Sie enthält die Authentifizierungsmethode für die Anmeldung sowie Details Auth (zum Beispiel: Telefon, SMS oder Voicemail) '
ms.openlocfilehash: a377c8648ebc8a6e3eb10fb6b0b87df066f8f2cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061419"
---
# <a name="mfadetail-resource-type"></a>Ressourcentyp mfaDetail
Gibt Details für eine bestimmte Anmeldung mehrstufiger Authentifizierung das an. Sie enthält die Authentifizierungsmethode für die Anmeldung sowie Details Auth (zum Beispiel: Telefon, SMS oder Voicemail) 



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|authDetail|String|Gibt an, für die entsprechende Aktivität-in den Details der mehrstufiger Authentifizierung das Auth der mehrstufiger Authentifizierung das erforderlich ist, "Yes".|
|Authentifizierungsmethode|String|Gibt die mehrstufiger Authentifizierung das Auth-Methoden (SMS, Telefon- und Authentifizierungsserver App sind einige der Wert) für die entsprechende Aktivität-Anmeldung bei das mehrstufiger Authentifizierung das erforderliche Feld ist "Yes" an.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->