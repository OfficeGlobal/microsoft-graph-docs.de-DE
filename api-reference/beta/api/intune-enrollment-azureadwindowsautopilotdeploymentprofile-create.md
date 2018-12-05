---
title: Erstellen von azureADWindowsAutopilotDeploymentProfile
description: Erstellen eines neuen AzureADWindowsAutopilotDeploymentProfile-Objekts.
ms.openlocfilehash: 7984dd9d1221ff27937fc366289b9c3f64ef20ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061049"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a>Erstellen von azureADWindowsAutopilotDeploymentProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Erstellen eines neuen [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekts.
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung für das Objekt AzureADWindowsAutopilotDeploymentProfile eine JSON-Darstellung.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AzureADWindowsAutopilotDeploymentProfile erstellen.

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
|extractHardwareHash|Boolesch|Extraktion von HardwareHash für das Profil Inherited aus [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|deviceNameTemplate|String|Die Vorlage verwendet, um das Gerät AutoPilot nennen. Dies kann ein benutzerdefinierter Text und kann auch die Seriennummer des Geräts, oder aber eine zufällig erzeugte Zahl enthalten. Die gesamte Länge des Texts von der Vorlage generierte kann nicht mehr als 15 Zeichen sein. Geerbt von [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1100

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1208

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value"
}
```




