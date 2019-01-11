---
title: Ressourcentyp activeDirectoryWindowsAutopilotDeploymentProfile
description: Windows Autopilot Bereitstellung Benutzerprofil
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a7928487cf0377407738e88f8a4da6a994cb0bba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866752"
---
# <a name="activedirectorywindowsautopilotdeploymentprofile-resource-type"></a>Ressourcentyp activeDirectoryWindowsAutopilotDeploymentProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows Autopilot Bereitstellung Benutzerprofil

Erbt vom [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste activeDirectoryWindowsAutopilotDeploymentProfiles](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-list.md)|[ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Auflistung|Listeneigenschaften und Beziehungen der [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekte.|
|[Abrufen von activeDirectoryWindowsAutopilotDeploymentProfile](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-get.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Lesen Sie Eigenschaften und Beziehungen des [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekts.|
|[Erstellen von activeDirectoryWindowsAutopilotDeploymentProfile](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-create.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Erstellen eines neuen [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekts.|
|[ActiveDirectoryWindowsAutopilotDeploymentProfile löschen](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-delete.md)|Keine|Löscht eine [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).|
|[ActiveDirectoryWindowsAutopilotDeploymentProfile aktualisieren](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-update.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Aktualisieren Sie die Eigenschaften eines [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Profil Schlüssel von [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) geerbt.|
|displayName|String|Name des Profils Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|description|String|Beschreibung des Profils Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|language|String|Auf dem Gerät Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) konfigurierten Sprache|
|createdDateTime|DateTimeOffset|Profil Erstellungszeit Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|lastModifiedDateTime|DateTimeOffset|Profil Zeitpunkt der letzten Änderung Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Out of Box experience Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) festlegen|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Registrierung Statusfenster Inherited aus [WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) festlegen|
|extractHardwareHash|Boolean|Extraktion von HardwareHash für das Profil Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|deviceNameTemplate|String|Die Vorlage verwendet, um das Gerät AutoPilot nennen. Dies kann ein benutzerdefinierter Text und kann auch die Seriennummer des Geräts, oder aber eine zufällig erzeugte Zahl enthalten. Die gesamte Länge des Texts von der Vorlage generierte kann nicht mehr als 15 Zeichen sein. Geerbt von [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignedDevices|[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Auflistung|Die Liste der Geräte für das Profil. Geerbt von [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|assignments|[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Auflistung|Die Liste der Gruppe Zuordnungen für das Profil. Geerbt von [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|domainJoinConfiguration|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Konfiguration in Active Directory-Domäne|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String"
}
```





