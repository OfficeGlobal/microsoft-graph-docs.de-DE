---
title: Ressourcentyp fileHash
description: Enthält Statusinformationen zu Dateihashes (cryptographic und der Speicherort).
localization_priority: Normal
ms.openlocfilehash: f5d865a7ded230ca611b8628c3648ec1e331c67d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815645"
---
# <a name="filehash-resource-type"></a>Ressourcentyp fileHash

Enthält Statusinformationen zu Dateihashes (cryptographic und der Speicherort).

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|hashType|[FileHashType](filehashtypeenumtype.md) -Enumeration|Hash-Dateityp. Mögliche Werte: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.|
|hashValue|String|Der Wert des Dateihash.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
