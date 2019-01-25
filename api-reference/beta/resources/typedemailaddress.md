---
title: Ressourcentyp typedEmailAddress
description: Stellt den Namen, e-Mail-Adressen und ihre entsprechenden e-Mail-Adresstyp eines Kontakts an.
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510708"
---
# <a name="typedemailaddress-resource-type"></a>Ressourcentyp typedEmailAddress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Namen, e-Mail-Adressen und ihre entsprechenden e-Mail-Adresstyp [wenden Sie sich an](contact.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|address|String|Die e-Mail-Adresse eines Kontakts.|
|name|Zeichenfolge|Der Anzeigename eines Kontakts.|
|type |String |Der Typ des e-Mail-Adresse. Mögliche Werte sind: `unknown`, `work`, `personal`, `main` und `other`. Der Standardwert ist `unknown`, d. h. **Adresse** wurde nicht als ein bestimmter Typ festgelegt. |
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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
