---
title: windowsAutopilotDeviceIdentity-Ressourcentyp
description: Die windowsAutopilotDeviceIdentity-Ressource stellt ein Windows Autopilot-Gerät dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63cb69d7d84940722b9a0436b65aa12efd0b7c72
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166381"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>windowsAutopilotDeviceIdentity-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die windowsAutopilotDeviceIdentity-Ressource stellt ein Windows Autopilot-Gerät dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsAutopilotDeviceIdentities aufListen](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekte.|
|[WindowsAutopilotDeviceIdentity abrufen](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Lesen von Eigenschaften und Beziehungen des [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[WindowsAutopilotDeviceIdentity erstellen](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Erstellen eines neuen [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[WindowsAutopilotDeviceIdentity löschen](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Keine|Löscht eine [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).|
|[WindowsAutopilotDeviceIdentity aktualisieren](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Aktualisieren der Eigenschaften eines [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[assignUserToDevice-Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Keine|Weist dem Benutzer Autopilot-Geräte zu.|
|[unassignUserFromDevice-Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Keine|Aufheben der Zuordnung des Benutzers zu einem Autopilot-Gerät.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|GUID des Objekts|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Profil Zuordnungsstatus des Windows Autopilot-Geräts. Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Profilzuweisung detaillierter Status des Windows Autopilot-Geräts. Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Festgelegte Zeit des Windows Autopilot-Geräts.|
|orderIdentifier|String|Auftragsbezeichner des Windows Autopilot-Geräts.|
|purchaseOrderIdentifier|Zeichenfolge|Bestellkennung des Windows Autopilot-Geräts.|
|serialNumber|String|Seriennummer des Windows AutoPilot-Geräts|
|productKey|Zeichenfolge|Product Key des Windows AutoPilot-Geräts|
|manufacturer|Zeichenfolge|OEM-Hersteller des Windows Autopilot-Geräts.|
|model|Zeichenfolge|Modellname des Windows Autopilot-Geräts.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|InTune-Registrierungsstatus des Windows Autopilot-Geräts. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|lastContactedDateTime|DateTimeOffset|InTune zuletzt kontaktierte Datum Uhrzeit des Windows Autopilot-Geräts.|
|addressableUserName|Zeichenfolge|Adressierbarer Benutzername.|
|userPrincipalName|Zeichenfolge|Benutzerprinzipal Name.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Bereitstellungsprofil, das dem Windows Autopilot-Gerät derzeit zugewiesen ist.|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Bereitstellungsprofil, das dem Windows Autopilot-Gerät zugewiesen werden soll.|

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




