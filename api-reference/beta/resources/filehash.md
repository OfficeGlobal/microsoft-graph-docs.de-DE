---
title: Ressourcentyp fileHash
description: Enthält Statusinformationen zu Dateihashes (cryptographic und der Speicherort).
ms.openlocfilehash: 8f283046efc9b4af181cb33fb4e9ca63e4892b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062396"
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