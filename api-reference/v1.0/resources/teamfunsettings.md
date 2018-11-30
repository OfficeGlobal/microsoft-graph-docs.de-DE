---
title: Ressourcentyp teamFunSettings
description: So konfigurieren Sie Einstellungen Verwenden von Giphy, Memes und Aufkleber im Team.
ms.openlocfilehash: ef816d027f015155cc09195c359523c83589725e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016408"
---
# <a name="teamfunsettings-resource-type"></a>Ressourcentyp teamFunSettings



Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowGiphy|Boolesch|Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.|
|giphyContentRating|Zeichenfolge (Aufzählung)|Giphy bewerten. Mögliche Werte sind: `moderate` und `strict`.|
|allowStickersAndMemes|Boolesch|Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.|
|allowCustomMemes|Boolesch|Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
