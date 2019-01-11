---
title: Ressourcentyp iosVppAppAssignedUserLicense
description: iOS-Lizenz von Benutzerrechten Volume Purchase Program. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.
localization_priority: Normal
ms.openlocfilehash: 3217fc338b2f0bb072de19cf0807a718a4998efa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806895"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>Ressourcentyp iosVppAppAssignedUserLicense

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

iOS-Lizenz von Benutzerrechten Volume Purchase Program. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.

Erbt vom [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Auflistung|Listeneigenschaften und Beziehungen der [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekte.|
|[Abrufen von iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Lesen Sie Eigenschaften und Beziehungen des [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.|
|[Erstellen von iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Erstellen eines neuen [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.|
|[IosVppAppAssignedUserLicense löschen](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|Keine|Löscht eine [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).|
|[IosVppAppAssignedUserLicense aktualisieren](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Aktualisieren Sie die Eigenschaften eines [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|Zeichenfolge|Die e-Mail-Adresse des Benutzers. Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|Zeichenfolge|Die Benutzer-ID. Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|Zeichenfolge|Der Benutzername. Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|Zeichenfolge|Der Benutzerprinzipalname. Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedUserLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





