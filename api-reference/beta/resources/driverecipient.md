---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ecf3e600cc943d0c82da38928d8018e6c654fb4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525801"
---
# <a name="driverecipient-resource"></a>DriveRecipient-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **DriveRecipient**-Ressource stellt eine Person, eine Gruppe oder einen anderen Empfänger für die Freigabe mit der [Einladen](../api/driveitem-invite.md)-Aktion dar.

## <a name="json-representation"></a>JSON-Darstellung

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a>Eigenschaften
Die Empfängerressource besitzt die folgenden Eigenschaften.

| Eigenschaftenname | Typ   | Beschreibung                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| E-Mail         | String | Die E-Mail-Adresse des Empfängers, wenn der Empfänger eine zugehörige E-Mail-Adresse aufweist.                  |
| Alias         | String | Der Alias des Domänenobjekts, für Fälle, in denen keine E-Mail-Adresse verfügbar ist (z. B. bei Sicherheitsgruppen). |
| objectId      | String | Der eindeutige Bezeichner für den Empfänger im Verzeichnis.                                               |

## <a name="remarks"></a>Bemerkungen

Bei Verwendung von [invite](../api/driveitem-invite.md) zum Hinzufügen von Berechtigungen kann im DriveRecipient **email**, **alias** oder **objectId** angegeben sein. Nur einer dieser Werte ist erforderlich.

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": [
    "Error: /api-reference/beta/resources/driverecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
