---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.openlocfilehash: f1bc78a8ec0648ce90221e4ad1f4473e49b625b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863728"
---
# <a name="driverecipient-resource"></a>DriveRecipient-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
