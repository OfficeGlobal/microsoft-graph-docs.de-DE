---
title: depEnrollmentProfile-Ressourcentyp
description: Die depEnrollmentProfile-Ressource stellt ein Registrierungsprofil für das Apple-Geräte Registrierungsprogramm (DEP) dar. Dieser Profiltyp muss Apple DEP-Seriennummern zugewiesen werden, bevor die entsprechenden Geräte über DEP registriert werden können.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ecc14dcd7cf2d171259c76592352ff13bb6ed1d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166423"
---
# <a name="depenrollmentprofile-resource-type"></a>depEnrollmentProfile-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die depEnrollmentProfile-Ressource stellt ein Registrierungsprofil für das Apple-Geräte Registrierungsprogramm (DEP) dar. Dieser Profiltyp muss Apple DEP-Seriennummern zugewiesen werden, bevor die entsprechenden Geräte über DEP registriert werden können.


Erbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DepEnrollmentProfiles aufListen](../api/intune-enrollment-depenrollmentprofile-list.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekte.|
|[DepEnrollmentProfile abrufen](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Lesen von Eigenschaften und Beziehungen des [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.|
|[DepEnrollmentProfile erstellen](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Erstellen eines neuen [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.|
|[DepEnrollmentProfile löschen](../api/intune-enrollment-depenrollmentprofile-delete.md)|Keine|Löscht eine [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).|
|[DepEnrollmentProfile aktualisieren](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Aktualisieren der Eigenschaften eines [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Die GUID für das von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Objekt.|
|displayName|Zeichenfolge|Name des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils|
|description|Zeichenfolge|Beschreibung des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils|
|requiresUserAuthentication|Boolean|Gibt an, ob für das Profil eine von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Benutzerauthentifizierung erforderlich ist.|
|configurationEndpointUrl|Zeichenfolge|Konfigurations Endpunkt-URL für die von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Registrierung|
|enableAuthenticationViaCompanyPortal|Boolean|Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll. Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten erforderlich ist, der von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbt wurde.|
|isDefault|Boolean|Gibt an, ob dies das Standardprofil ist.|
|supervisedModeEnabled|Boolean|Überwachter Modus, true, um zu aktivieren, andernfalls false. Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter.|
|supportDepartment|Zeichenfolge|Informationen zur Support Abteilung|
|passCodeDisabled|Boolean|Gibt an, ob der Bereich "Passcode" deaktiviert ist.|
|isMandatory|Boolean|Gibt an, ob das Profil obligatorisch ist.|
|locationDisabled|Boolean|Gibt an, ob der Standortdienst-Setup Bereich deaktiviert ist.|
|supportPhoneNumber|Zeichenfolge|Support-Telefonnummer|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Gibt den iTunes-paarungsmodus an. Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.|
|profileRemovalDisabled|Boolean|Gibt an, ob die Profil Entfernungs Option deaktiviert ist.|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Sammlung|Verwaltungszertifikate für Apple Configurator|
|restoreBlocked|Boolean|Gibt an, ob der wiederHerstellungs-Setup Bereich blockiert ist|
|restoreFromAndroidDisabled|Boolean|Gibt an, ob die Wiederherstellung von Android deaktiviert ist.|
|appleIdDisabled|Boolean|Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist.|
|termsAndConditionsDisabled|Boolean|Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist.|
|touchIdDisabled|Boolean|Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist.|
|applePayDisabled|Boolean|Gibt an, ob der Apple Pay-Setup Bereich deaktiviert ist.|
|zoomDisabled|Boolean|Gibt an, ob der Zoom-Setup Bereich deaktiviert ist.|
|siriDisabled|Boolean|Gibt an, ob der Siri-Setup Bereich deaktiviert ist.|
|diagnosticsDisabled|Boolean|Gibt an, ob der Diagnose-Setup Bereich deaktiviert ist.|
|macOSRegistrationDisabled|Boolean|Gibt an, ob die Mac OS-Registrierung deaktiviert ist.|
|macOSFileVaultDisabled|Boolean|Gibt an, ob das Mac OS-Dateidepot deaktiviert ist.|
|awaitDeviceConfiguredConfirmation|Boolean|Gibt an, ob das Gerät auf die konfigurierte Bestätigung warten muss.|
|sharedIPadMaximumUserCount|Int32|Dies gibt die maximale Anzahl von Benutzern an, die ein freigegebenes iPad verwenden können. Gilt nur für den freigegebenen iPad-Modus.|
|Enablesharedipad wurden|Boolean|Dieser Wert gibt an, ob das Gerät in einen Modus eingeschrieben werden soll, der mehrere Benutzerszenarien ermöglicht. Gilt nur für freigegebene iPads.|

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
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
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




