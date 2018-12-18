---
title: Ressourcentyp depEnrollmentProfile
description: Die Ressource DepEnrollmentProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können
author: tfitzmac
ms.openlocfilehash: 5079a109e2c1aa236c69fff8d114e4a37d82367c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316968"
---
# <a name="depenrollmentprofile-resource-type"></a>Ressourcentyp depEnrollmentProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource DepEnrollmentProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können

Erbt vom [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Auflistung|Listeneigenschaften und Beziehungen der [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekte.|
|[Abrufen von depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Lesen Sie Eigenschaften und Beziehungen des [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.|
|[Erstellen von depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Erstellen eines neuen [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.|
|[DepEnrollmentProfile löschen](../api/intune-enrollment-depenrollmentprofile-delete.md)|Keines|Löscht eine [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).|
|[DepEnrollmentProfile aktualisieren](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Aktualisieren Sie die Eigenschaften eines [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolesch|Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert|
|configurationEndpointUrl|String|Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration|
|enableAuthenticationViaCompanyPortal|Boolesch|Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal. Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolescher Wert|Gibt an, ob dies das Standardprofil ist|
|supervisedModeEnabled|Boolesch|Überwachten Modus aktivieren, False andernfalls True. Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.|
|supportDepartment|String|Abteilung Supportinformationen|
|passCodeDisabled|Boolesch|Gibt an, ob Kennung Setup Bereich deaktiviert ist|
|isMandatory|Boolesch|Gibt an, ob das Profil zwingend erforderlich ist.|
|locationDisabled|Boolesch|Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist|
|supportPhoneNumber|String|Support-Telefonnummer|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Gibt den Modus Paarung iTunes an. Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.|
|profileRemovalDisabled|Boolesch|Gibt an, ob die Option Profil entfernen deaktiviert ist|
|managementCertificates|[ManagementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Auflistung|Verwaltung von Zertifikaten für Apple-Konfiguration|
|restoreBlocked|Boolesch|Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist|
|restoreFromAndroidDisabled|Boolesch|Gibt an, ob die Wiederherstellung von Android deaktiviert ist|
|appleIdDisabled|Boolesch|Gibt an, ob Apple Id Setup Bereich deaktiviert ist|
|termsAndConditionsDisabled|Boolesch|Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist|
|touchIdDisabled|Boolesch|Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist|
|applePayDisabled|Boolesch|Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist|
|zoomDisabled|Boolesch|Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist|
|siriDisabled|Boolesch|Gibt an, ob Siri Setup Bereich deaktiviert ist|
|diagnosticsDisabled|Boolesch|Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist|
|macOSRegistrationDisabled|Boolesch|Gibt an, ob Mac OS-Registrierung deaktiviert ist|
|macOSFileVaultDisabled|Boolesch|Gibt an, ob die Datei Vault Mac OS deaktiviert ist|
|awaitDeviceConfiguredConfirmation|Boolesch|Gibt an, ob das Gerät konfigurierten Bestätigung warten müssen|
|sharedIPadMaximumUserCount|Int32|Dies gibt die maximale Anzahl von Benutzern, die eine freigegebene iPad verwenden können. Gilt nur im freigegebenen iPad-Modus.|
|enableSharedIPad|Boolesch|Dies gibt an, ob das Gerät in einen Modus registriert werden, wodurch Multi-Benutzerszenarien. Nur im freigegebenen iPads anwendbar.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```





