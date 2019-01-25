---
title: internetMessageHeader-Ressourcentyp
description: 'Schlüssel-Wert-Paar, die eine Internet-Nachrichtenkopfzeile darstellt, wie durch RFC5322, definiert, die bereitstellt '
localization_priority: Normal
ms.openlocfilehash: e748e6badd3e6bad6adb02a9df46a40a7241d636
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511667"
---
# <a name="internetmessageheader-resource-type"></a>internetMessageHeader-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Schlüssel-Wert-Paar, das eine Internet-Nachrichtenkopfzeile darstellt, wie von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) definiert, die Informationen zum Netzwerkpfad einer Nachricht vom Absender bis zum Empfänger liefert. 

Beispiele für eine Internet-Nachrichtenkopfzeile finden Sie unter [Anzeigen E-Mail-Kopfzeilen](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|string|Stellt den Schlüssel in einem Schlüssel-Wert-Paar dar.|
|Wert|string|Der Wert in einem Schlüssel-Wert-Paar.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/internetmessageheader.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
