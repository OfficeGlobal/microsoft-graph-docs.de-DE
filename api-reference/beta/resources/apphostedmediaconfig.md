---
title: Ressourcentyp appHostedMediaConfig
description: Medienstapel, die von der Anwendung gehostet wird.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 583964a6c7cd65ae4e8341f7fcba92d754916b36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884567"
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
