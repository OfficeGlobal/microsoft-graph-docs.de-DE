---
title: DepIOSEnrollmentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DepIOSEnrollmentProfile-Objekts.
ms.openlocfilehash: 75fbf56532a4145537b714a73626dd01554179a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063816"
---
# <a name="update-depiosenrollmentprofile"></a>DepIOSEnrollmentProfile aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren Sie die Eigenschaften eines [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.
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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung für das Objekt [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) eine JSON-Darstellung.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolesch|Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert|
|configurationEndpointUrl|String|Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration|
|enableAuthenticationViaCompanyPortal|Boolesch|Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal. Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolescher Wert|Gibt an, ob dies das Standardprofil Inherited aus [DepEnrollmentBaseProfile ist](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boolesch|Überwachten Modus aktivieren, False andernfalls True. Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen. Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|Supportinformationen Sie Abteilung Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|passCodeDisabled|Boolesch|Gibt an, ob Kennung Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert|
|isMandatory|Boolesch|Gibt an, ob das Profil obligatorisch Inherited aus [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Boolesch|Gibt an, ob der Dienst Setup Bereich ist Speicherort Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert|
|supportPhoneNumber|String|Unterstützung der Telefonnummer Inherited von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolesch|Gibt an, ob die Option Profil entfernen deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt|
|restoreBlocked|Boolesch|Gibt an, ob die Wiederherstellung Setup Bereich ausgeschlossen wird von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt|
|appleIdDisabled|Boolesch|Gibt an, ob Apple Id Setup Bereich ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert|
|termsAndConditionsDisabled|Boolesch|Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt|
|touchIdDisabled|Boolesch|Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt|
|applePayDisabled|Boolesch|Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt|
|zoomDisabled|Boolesch|Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt|
|siriDisabled|Boolesch|Gibt an, ob Siri Setup Bereich deaktiviert ist von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt|
|diagnosticsDisabled|Boolesch|Gibt an, ob die Diagnose, den Bereich Setup ist Inherited von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) deaktiviert|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Gibt den Modus Paarung iTunes an. Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.|
|managementCertificates|[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung|Verwaltung von Zertifikaten für Apple-Konfiguration|
|restoreFromAndroidDisabled|Boolesch|Gibt an, ob die Wiederherstellung von Android deaktiviert ist|
|awaitDeviceConfiguredConfirmation|Boolesch|Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen|
|sharedIPadMaximumUserCount|Int32|Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können. Gilt nur im freigegebenen iPad-Modus.|
|enableSharedIPad|Boolesch|Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien. Nur im freigegebenen iPads anwendbar.|
|companyPortalVppTokenId|String|Wenn festgelegt ist, gibt an, welche Vpp Token zum Bereitstellen der Unternehmensportal mit Gerät-Lizenzierung verwendet werden soll. 'EnableAuthenticationViaCompanyPortal' muss für diese Eigenschaft festgelegt werden soll festgelegt sein.|
|enableSingleAppEnrollmentMode|Boolesch|Weist das Gerät zum Aktivieren der einzelnen app-Modus und Anwenden von app-Sperre während der Registrierung. Standard ist false. 'EnableAuthenticationViaCompanyPortal' und 'CompanyPortalVppTokenId' müssen für diese Eigenschaft festgelegt werden soll, festgelegt werden.|



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1267

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1378

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true
}
```





