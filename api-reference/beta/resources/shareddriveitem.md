---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 22e449d725b94b7be458261e82cfde0b5d6fdf9c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524121"
---
# <a name="shareddriveitem-resource-type"></a>SharedDriveItem-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **sharedDriveItem**-Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares-get.md)-API für den Zugriff auf ein freigegebenes[driveItem](driveitem.md)-Objekt verwendet wird.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **sharedDriveItem**-Ressource.

Die **sharedDriveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "permission": { "@odata.type": "microsoft.graph.permission" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ                          | Beschreibung                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | String                        | Die eindeutige ID der Freigabe, auf die zugegriffen wird.              |
| name     | String                        | Der Anzeigename für das freigegebene Element.                             |
| owner    | [IdentitySet](identityset.md) | Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird. |

## <a name="relationships"></a>Beziehungen

| Beziehungsname | Typ                | Beschreibung
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem] | Dient für den Zugriff auf das zugrunde liegende **driveItem**
| **list**          | [**list**][list]           | Dient für den Zugriff auf das zugrunde liegende **list**
| **listItem**      | [**listItem**][listItem]   | Dient für den Zugriff auf das zugrunde liegende **listItem**
| **permission**    | Berechtigung | Verwendet, um die **Berechtigung** für den zugrunde liegenden sharing Hyperlink zugreifen
| **site**          | [**site**][site]           | Dient für den Zugriff auf das zugrunde liegende **site**

Für in persönlichen OneDrive-Konten freigegebene **driveItems** könnenSie alternativ ebenfalls folgende Beziehungen verwenden.

| Beziehungsname | Typ                         | Beschreibung
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**driveItem**][driveItem]-Sammmlung | Alle im Freigabestamm enthaltenen driveItems. Diese Sammlung kann nicht aufgezählt werden.
| **driveItem**     | [**driveItem**][driveItem]            | Dient für den Zugriff auf das zugrunde liegende **driveItem**

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a>Methoden

| Methode                                  | REST-Pfad                |
| :-------------------------------------- | :----------------------- |
| [Freigegebenes Element abrufen](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": [
    "Error: /api-reference/beta/resources/shareddriveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
