---
title: FileHashType-Enumeration
description: Enum für Hash Dateitypen.
localization_priority: Normal
ms.openlocfilehash: 082fdd9cdad6c3ec1ea4e07020983ac0bac7ed65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518380"
---
# <a name="filehashtype-enum"></a>FileHashType-Enumeration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enum für Hash Dateitypen.

## <a name="members"></a>Elemente

|Member|Wert|Beschreibung|
|:---|:---|:---|
|unknown|(0)|Unbekannten Typs.|
|SHA1|-1|SHA1 Hash-Typ.|
|SHA256|-2| SHA256-Hash-Typ.|
|MD5|-3| MD5 Hash-Typ.|
|authenticodeHash256|4*| AuthenticodeHash256 Hash-Typ.|
|lsHash|$-5| LsHash Hash-Typ.|
|ctph|-6| CTPH Hash-Typ.|
|peSha1|-7| PESHA1 Hash-Typ.|
|peSha256|8*| PESHA256 Hash-Typ.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filehashtypeenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
