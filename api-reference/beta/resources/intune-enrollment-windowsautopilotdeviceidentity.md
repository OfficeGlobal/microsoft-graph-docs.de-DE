---
title: Ressourcentyp windowsAutopilotDeviceIdentity
description: Die Ressource WindowsAutopilotDeviceIdentity stellt ein Windows-Autopilot-Gerät.
ms.openlocfilehash: 82ce93928e90d3649dd11d32cb8609254533315b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064262"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Ressourcentyp windowsAutopilotDeviceIdentity

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource WindowsAutopilotDeviceIdentity stellt ein Windows-Autopilot-Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekte.|
|[Abrufen von windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[Erstellen von windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Erstellen eines neuen [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[WindowsAutopilotDeviceIdentity löschen](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Keines|Löscht eine [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).|
|[WindowsAutopilotDeviceIdentity aktualisieren](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[AssignUserToDevice Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Keines|Autopilot Geräte Benutzer zugewiesen.|
|[UnassignUserFromDevice Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Keines|Die Benutzer von einem Gerät Autopilot unassigns.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Profil Zuordnungsstatus des Geräts Autopilot Windows. Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Profil Zuordnung detaillierter Status des Geräts Autopilot Windows. Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Profil festlegen Uhrzeit des Geräts Autopilot Windows.|
|orderIdentifier|String|Die Kennung des Geräts Autopilot Windows.|
|purchaseOrderIdentifier|String|Kennung des Geräts Autopilot Windows Bestellung.|
|serialNumber|String|Seriennummer des Windows AutoPilot-Geräts|
|productKey|String|Product Key des Windows AutoPilot-Geräts|
|manufacturer|String|OEM-Hersteller des Geräts Autopilot Windows.|
|model|String|Modellname des Geräts Autopilot Windows.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Registrierung-Zustand des Geräts Autopilot Windows Intune. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|lastContactedDateTime|DateTimeOffset|Intune kontaktiert Datum Uhrzeit der letzten des Geräts Autopilot Windows.|
|addressableUserName|String|Adressierbaren Benutzername.|
|userPrincipalName|String|Benutzerprinzipalname.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Bereitstellungsprofil das Windows Autopilot Gerät derzeit zugewiesen sind.|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Bereitstellungsprofil vorgesehen, die Windows-Gerät Autopilot zugewiesen werden soll.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "deploymentProfileAssignmentStatus": "String",
  "deploymentProfileAssignmentDetailedStatus": "String",
  "deploymentProfileAssignedDateTime": "String (timestamp)",
  "orderIdentifier": "String",
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String"
}
```





