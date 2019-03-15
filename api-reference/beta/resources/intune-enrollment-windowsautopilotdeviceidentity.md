---
title: windowsAutopilotDeviceIdentity-Ressourcentyp
description: Die windowsAutopilotDeviceIdentity-Ressource stellt ein Windows Autopilot-Gerät dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4eaa6f948354164debd73793524d047b1ba204fd
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571438"
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
|[WindowsAutopilotDeviceIdentity löschen](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|None|Löscht eine [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).|
|[WindowsAutopilotDeviceIdentity aktualisieren](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Aktualisieren der Eigenschaften eines [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.|
|[assignUserToDevice-Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|None|Weist dem Benutzer Autopilot-Geräte zu.|
|[unassignUserFromDevice-Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|None|Aufheben der Zuordnung des Benutzers zu einem Autopilot-Gerät.|
|[assignResourceAccountToDevice-Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|None|Weist den Autopilot-Geräten ein Ressourcenkonto zu.|
|[unassignResourceAccountFromDevice-Aktion](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|None|Aufheben der Zuweisung des Ressourcenkontos von einem Autopilot-Gerät.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|GUID des Objekts|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Profil Zuordnungsstatus des Windows Autopilot-Geräts. Mögliche Werte: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Profilzuweisung detaillierter Status des Windows Autopilot-Geräts. Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Festgelegte Zeit des Windows Autopilot-Geräts.|
|orderIdentifier|String|Auftragsbezeichner des Windows Autopilot-Geräts.|
|purchaseOrderIdentifier|String|Bestellkennung des Windows Autopilot-Geräts.|
|serialNumber|String|Seriennummer des Windows AutoPilot-Geräts|
|productKey|String|Product Key des Windows AutoPilot-Geräts|
|Hersteller|String|OEM-Hersteller des Windows Autopilot-Geräts.|
|model|String|Modellname des Windows Autopilot-Geräts.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|InTune-Registrierungsstatus des Windows Autopilot-Geräts. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|lastContactedDateTime|DateTimeOffset|InTune zuletzt kontaktierte Datum Uhrzeit des Windows Autopilot-Geräts.|
|addressableUserName|String|Adressierbarer Benutzername.|
|userPrincipalName|String|Benutzerprinzipal Name.|
|resourceName|String|Ressourcen Name.|
|skuNumber|String|SKU-Nummer|
|systemFamily|String|System Familie|
|Eigenschaften azureactivedirectorydeviceid|String|AAD-Geräte-ID|
|managedDeviceId|String|Verwaltete Geräte-ID|

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
  "userPrincipalName": "String",
  "resourceName": "String",
  "skuNumber": "String",
  "systemFamily": "String",
  "azureActiveDirectoryDeviceId": "String",
  "managedDeviceId": "String"
}
```




