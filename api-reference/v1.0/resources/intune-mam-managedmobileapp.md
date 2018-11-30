---
title: managedMobileApp-Ressourcentyp
description: Der Bezeichner für die Bereitstellung einer App
ms.openlocfilehash: 7915ef27dccfeef681475161261f36b64b79ff23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020043"
---
# <a name="managedmobileapp-resource-type"></a>managedMobileApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der Bezeichner für die Bereitstellung einer App
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedMobileApps auflisten](../api/intune-mam-managedmobileapp-list.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekte.|
|[managedMobileApp abrufen](../api/intune-mam-managedmobileapp-get.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Lesen von Eigenschaften und Beziehungen des [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekts.|
|[managedMobileApp erstellen](../api/intune-mam-managedmobileapp-create.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Erstellen eines neuen [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekts.|
|[managedMobileApp löschen](../api/intune-mam-managedmobileapp-delete.md)|Keine|Löscht ein [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekt.|
|[managedMobileApp aktualisieren](../api/intune-mam-managedmobileapp-update.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Aktualisieren der Eigenschaften eines [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Bezeichner der App mit dem zugehörigen Betriebssystemtyp|
|id|String|Schlüssel der Entität|
|Version|String|Version der Entität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



