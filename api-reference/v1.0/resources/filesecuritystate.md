---
title: Ressourcentyp fileSecurityState
description: Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894096"
---
# <a name="filesecuritystate-resource-type"></a>Ressourcentyp fileSecurityState

Enthält Informationen zur Datei (nicht verarbeiten) im Zusammenhang mit der Benachrichtigung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).|
|name|Zeichenfolge|Der Dateiname (ohne Pfad).|
|Pfad|Zeichenfolge|Vollständiger Dateipfad der die Datei/ImageFile.|
|riskScore|Zeichenfolge|Anbieter generiert/berechnet riskieren Bewertung der alert-Datei. Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
