---
title: Ressourcentyp appHostedMediaConfig
description: Medienstapel, die von der Anwendung gehostet wird.
author: VinodRavichandran
ms.openlocfilehash: b96d6ff836ab36e5561c9ba3958123178e2fbde9
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380128"
---
# <a name="apphostedmediaconfig-resource-type"></a>Ressourcentyp appHostedMediaConfig

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Medienstapel, die von der Anwendung gehostet wird.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                          | Typ    | Beschreibung                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| BLOB                              | Zeichenfolge  | Die Medien Konfiguration Blob vom smart Media-Agent generiert.    |
| removeFromDefaultAudioGroup       | Boolescher Wert | Entfernen von Audio aus der Standardgruppe audio                       |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appHostedMediaConfig"
}-->
```json
{
  "blob": "String",
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
