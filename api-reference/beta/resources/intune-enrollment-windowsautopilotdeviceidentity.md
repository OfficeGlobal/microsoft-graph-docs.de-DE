---
title: Ressourcentyp windowsAutopilotDeviceIdentity
description: Die Ressource WindowsAutopilotDeviceIdentity stellt ein Windows-Autopilot-Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e69f93aff041f99728a224ce6e50a5e711919b1e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423923"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Ressourcentyp windowsAutopilotDeviceIdentity

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Ressource WindowsAutopilotDeviceIdentity stellt ein Windows-Autopilot-Gerät.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekte.|
|[Abrufen von windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[Erstellen von windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Erstellen eines neuen [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[WindowsAutopilotDeviceIdentity löschen](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Keine|Löscht eine [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).|
|[WindowsAutopilotDeviceIdentity aktualisieren](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[AssignUserToDevice Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Keine|Autopilot Geräte Benutzer zugewiesen.|
|[UnassignUserFromDevice Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Keine|Die Benutzer von einem Gerät Autopilot unassigns.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Profil Zuordnungsstatus des Geräts Autopilot Windows. Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Profil Zuordnung detaillierter Status des Geräts Autopilot Windows. Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Profil festlegen Uhrzeit des Geräts Autopilot Windows.|
|orderIdentifier|String|Die Kennung des Geräts Autopilot Windows.|
|purchaseOrderIdentifier|Zeichenfolge|Kennung des Geräts Autopilot Windows Bestellung.|
|serialNumber|String|Seriennummer des Windows AutoPilot-Geräts|
|productKey|String|Product Key des Windows AutoPilot-Geräts|
|manufacturer|Zeichenfolge|OEM-Hersteller des Geräts Autopilot Windows.|
|model|Zeichenfolge|Modellname des Geräts Autopilot Windows.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Registrierung-Zustand des Geräts Autopilot Windows Intune. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|lastContactedDateTime|DateTimeOffset|Intune kontaktiert Datum Uhrzeit der letzten des Geräts Autopilot Windows.|
|addressableUserName|Zeichenfolge|Adressierbaren Benutzername.|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname.|

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




