---
title: Ressourcentyp iosVppAppAssignedLicense
description: iOS Volume Purchase Program lizenzzuweisung. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.
ms.openlocfilehash: f1083934844f808c2630ecaeaa195734235e2a55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065467"
---
# <a name="iosvppappassignedlicense-resource-type"></a>Ressourcentyp iosVppAppAssignedLicense

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

iOS Volume Purchase Program lizenzzuweisung. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Auflistung|Listeneigenschaften und Beziehungen der [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekte.|
|[Abrufen von iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Lesen Sie Eigenschaften und Beziehungen des [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|
|[Erstellen von iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Erstellen eines neuen [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|
|[IosVppAppAssignedLicense löschen](../api/intune-apps-iosvppappassignedlicense-delete.md)|Keines|Löscht eine [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[IosVppAppAssignedLicense aktualisieren](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Aktualisieren Sie die Eigenschaften eines [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|userEmailAddress|String|Die e-Mail-Adresse des Benutzers.|
|userId|String|Die Benutzer-ID.|
|userName|String|Der Benutzername.|
|userPrincipalName|String|Der Benutzerprinzipalname.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





