---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 0f3acc102762cc1243d8be8362149df1d33717dc
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482042"
---
# <a name="sharinginvitation-resource-type"></a>SharingInvitation-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **SharingInvitation**-Ressource gruppiert Datenelemente im Zusammenhang mit einer Einladung in einer einzelnen Struktur.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname  | Typ                          | Beschreibung                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| E-Mail          | String                        | Die für den Empfänger der Freigabeeinladung angegebene E-Mail-Adresse. Schreibgeschützt.                                          |
| invitedBy      | [identitySet](identityset.md) | Stellt Informationen zum Absender der Einladung bereit, der diese Berechtigung erstellt hat, wenn diese Informationen verfügbar sind. Schreibgeschützt. |
| signInRequired | Boolean                       | Bei `true` muss sich der Empfänger der Einladung anmelden, um auf das freigegebene Element zugreifen zu können. Schreibgeschützt.                     |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinginvitation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
