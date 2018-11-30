---
title: Ressourcentyp typedEmailAddress
description: Stellt den Namen, e-Mail-Adressen und ihre entsprechenden e-Mail-Adresstyp eines Kontakts an.
ms.openlocfilehash: 3f40add32fbc219606b6d78041552fc108803d1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066073"
---
# <a name="typedemailaddress-resource-type"></a>Ressourcentyp typedEmailAddress

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt den Namen, e-Mail-Adressen und ihre entsprechenden e-Mail-Adresstyp [wenden Sie sich an](contact.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|address|String|Die e-Mail-Adresse eines Kontakts.|
|name|String|Der Anzeigename eines Kontakts.|
|Typ |String |Der Typ des e-Mail-Adresse. Mögliche Werte sind: `unknown`, `work`, `personal`, `main` und `other`. Der Standardwert ist `unknown`, d. h. **Adresse** wurde nicht als ein bestimmter Typ festgelegt. |
|otherLabel |String  |Wenn Sie einen benutzerdefinierten Typ des e-Mail-Adresse angeben, legen Sie **Typ** auf `other`, und weisen Sie eine benutzerdefinierte Zeichenfolge **OtherLabel** . Beispielsweise können Sie eine bestimmte e-Mail-Adresse für Ihre freiwillige Aktivitäten. Legen Sie **Typ** `other`, und legen Sie **OtherLabel** auf eine benutzerdefinierte Zeichenfolge wie `Volunteer work`. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
