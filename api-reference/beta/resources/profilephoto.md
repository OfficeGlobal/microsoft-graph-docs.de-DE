---
title: profilePhoto-Ressourcentyp
description: Ein Profilfoto von einem Benutzer, Gruppe oder ein Outlook-Kontakt auf die in Exchange Online oder Azure Active Directory (AAD) zugegriffen. Es ist nicht im Base64-codierte Binärdaten.
localization_priority: Normal
ms.openlocfilehash: 2a831abd098fb9a0dfa95f6d6dd3a9cd5de128cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513655"
---
# <a name="profilephoto-resource-type"></a>profilePhoto-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Profilfoto von einem Benutzer, Gruppe oder ein Outlook-Kontakt auf die in Exchange Online oder Azure Active Directory (AAD) zugegriffen. Es ist nicht im Base64-codierte Binärdaten.

Die unterstützten Größen der HD-Fotos auf Exchange Online sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“. Klicken Sie auf AAD können Fotos alle Dimension sein.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[profilePhoto abrufen](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |Rufen Sie die angegebenen **ProfilePhoto** oder der Metadaten (**ProfilePhoto** Eigenschaften). |
|[Update](../api/profilephoto-update.md) | [profilePhoto](profilephoto.md)  |Weist dem angegebenen Benutzer, der angegebenen Gruppe oder dem angegebenen Kontakt ein Foto zu. Das Foto sollte binär sein. Es ersetzt vorhandene Fotos (falls vorhanden). |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Schreibgeschützt.|
|height|int32|Die Höhe des Fotos. Schreibgeschützt.|
|width|int32|Die Breite des Fotos. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/profilephoto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
