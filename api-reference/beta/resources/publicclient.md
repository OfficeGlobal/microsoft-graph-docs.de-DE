---
title: Ressourcentyp publicClient
description: Gibt die Einstellungen für nicht Web App oder Web-Api. (Mobile oder anderen öffentlichen Client wie eine installierte Anwendung, die auf einem Desktopgerät ausgeführt)
localization_priority: Normal
ms.openlocfilehash: ff1d77709293a7167868451671e1660196c9a4db
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525962"
---
# <a name="publicclient-resource-type"></a>Ressourcentyp publicClient

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt die Einstellungen für nicht Web App oder Web-Api. (Mobile oder anderen öffentlichen Client wie eine installierte Anwendung, die auf einem Desktopgerät ausgeführt)

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|redirectUris|Zeichenfolgenauflistung| Gibt die URLs der Benutzertoken für die Anmeldung an gesendet werden, oder die Umleitung, URIs, dass OAuth 2.0 Autorisierungscodes und Zugriffstoken gesendet werden. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
