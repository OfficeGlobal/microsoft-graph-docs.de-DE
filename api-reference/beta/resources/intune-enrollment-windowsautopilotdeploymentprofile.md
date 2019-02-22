---
title: Windowsautopilotdeploymentprofile hinzugefügt-Ressourcentyp
description: Windows Autopilot-BereitstellungsProfil
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3b815e0184ab9969af348338c07c3fabf0b0597
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168873"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>Windowsautopilotdeploymentprofile hinzugefügt-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Windows Autopilot-BereitstellungsProfil

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Windowsautopilotdeploymentprofile hinzugefügt abrufen](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Lesen von Eigenschaften und Beziehungen des [windowsautopilotdeploymentprofile hinzugefügt](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) -Objekts.|
|[assign-Aktion](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Profilschlüssel|
|displayName|Zeichenfolge|Name des Profils|
|description|Zeichenfolge|Beschreibung des Profils|
|language|Zeichenfolge|Auf dem Gerät konfigurierte Sprache|
|createdDateTime|DateTimeOffset|Erstellungszeit für profile|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt der letzten Änderung des Profils|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Einstellung für die Out-of-Box-Erfahrung|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Einstellung für den Registrierungsstatus|
|extractHardwareHash|Boolescher Wert|HardwareHash-Extraktion für das Profil|
|deviceNameTemplate|Zeichenfolge|Die Vorlage, die zum Benennen des autoPilot-Geräts verwendet wird. Dabei kann es sich um einen benutzerdefinierten Text handeln, der entweder die Seriennummer des Geräts oder eine zufällig generierte Zahl enthalten kann. Die Gesamtlänge des von der Vorlage generierten Texts darf nicht mehr als 15 Zeichen betragen.|
|enableWhiteGlove|Boolescher Wert|Aktivieren Sie den weißen Handschuh Autopilot für das Profil.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignedDevices|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Sammlung|Die Liste der zugewiesenen Geräte für das Profil.|
|assignments|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Sammlung|Die Liste der Gruppenzuweisungen für das Profil.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
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
  "deviceNameTemplate": "String",
  "enableWhiteGlove": true
}
```




