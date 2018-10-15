---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: abcf686be46e15a523a1a88170981cb318e71b00
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268200"
---
# <a name="shareddriveitem-resource-type"></a>SharedDriveItem-Ressourcentyp

Die **sharedDriveItem**-Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares_get.md)-API für den Zugriff auf ein freigegebenes[driveItem](driveitem.md)-Objekt verwendet wird.

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
| ID       | Zeichenfolge                        | Die eindeutige ID der Freigabe, auf die zugegriffen wird.              |
| name     | Zeichenfolge                        | Der Anzeigename für das freigegebene Element.                             |
| Besitzer    | [IdentitySet](identityset.md) | Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird. |

## <a name="relationships"></a>Beziehungen

| Beziehungsname | Typ                | Beschreibung
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | Dient für den Zugriff auf das zugrunde liegende **driveItem**
| **Liste**          | [**list**][list]        | Dient für den Zugriff auf das zugrunde liegende **list**
| **listItem**      | [**listItem**][listItem]    | Dient für den Zugriff auf das zugrunde liegende **listItem**
| **site**          | [**site**][site]        | Dient für den Zugriff auf das zugrunde liegende **site**

Für in persönlichen OneDrive-Konten freigegebene **driveItems** könnenSie alternativ ebenfalls folgende Beziehungen verwenden.

| Beziehungsname | Typ                         | Beschreibung
| ------------------|:-----------------------------|:-----------------------------------
| **Positionen**         | [**driveItem**][driveItem]-Sammmlung | Alle im Freigabestamm enthaltenen driveItems. Diese Sammlung kann nicht aufgezählt werden.
| **root**          | [**driveItem**][driveItem]   | Dient dem Zugriff auf das zugrunde liegende **driveItem**. Veraltet – verwenden Sie `driveItem` stattdessen.

[driveItem]: driveItem.md
[list]: list.md
[listItem]: listItem.md
[site]: site.md

## <a name="methods"></a>Methods

| Methode                                  | REST-Pfad                |
| :-------------------------------------- | :----------------------- |
| [Freigegebenes Element abrufen](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
