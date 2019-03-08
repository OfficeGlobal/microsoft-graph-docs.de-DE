---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 0d0c5a34d12fe467196c0616befc7376835b632c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481727"
---
# <a name="shareddriveitem-resource-type"></a>SharedDriveItem-Ressourcentyp

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
| **driveItem**     | [**driveItem**][driveItem]   | Dient für den Zugriff auf das zugrunde liegende **driveItem**
| **list**          | [**list**][list]        | Dient für den Zugriff auf das zugrunde liegende **list**
| **listItem**      | [**listItem**][listItem]    | Dient für den Zugriff auf das zugrunde liegende **listItem**
| **site**          | [**site**][site]        | Dient für den Zugriff auf das zugrunde liegende **site**

Für in persönlichen OneDrive-Konten freigegebene **driveItems** könnenSie alternativ ebenfalls folgende Beziehungen verwenden.

| Beziehungsname | Typ                         | Beschreibung
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**driveItem**][driveItem]-Sammmlung | Alle im Freigabestamm enthaltenen driveItems. Diese Sammlung kann nicht aufgezählt werden.
| **root**          | [**driveItem**][driveItem]   | Wird für den Zugriff auf die zugrunde liegenden **DriveItem**verwendet. Veraltet-verwenden Sie `driveItem` stattdessen.

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a>Methoden

| Methode                                  | REST-Pfad                |
| :-------------------------------------- | :----------------------- |
| [Freigegebenes Element abrufen](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
