---
title: Ressourcentyp appHostedMediaConfig
description: Medienstapel, die von der Anwendung gehostet wird.
ms.openlocfilehash: 39080a8fdb5688ed9f1a5a8daba43266a0e7003e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059439"
---
# <a name="apphostedmediaconfig-resource-type"></a>Ressourcentyp appHostedMediaConfig

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Medienstapel, die von der Anwendung gehostet wird.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                          | Typ    | Beschreibung                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| BLOB                              | String  | Die Medien Konfiguration Blob vom smart Media-Agent generiert.    |
| removeFromDefaultAudioGroup       | Boolesch | Entfernen von Audio aus der Standardgruppe audio                       |

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
