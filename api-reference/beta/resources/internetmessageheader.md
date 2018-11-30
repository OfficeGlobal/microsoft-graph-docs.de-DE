---
title: internetMessageHeader-Ressourcentyp
description: 'Schlüssel-Wert-Paar, die eine Internet-Nachrichtenkopfzeile darstellt, wie durch RFC5322, definiert, die bereitstellt '
ms.openlocfilehash: 420d39b6a139563e3f5f277f032f0f7a29252337
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061244"
---
# <a name="internetmessageheader-resource-type"></a>internetMessageHeader-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->