---
title: depIOSEnrollmentProfile-Ressourcentyp
description: Die DepIOSEnrollmentProfile-Ressource stellt ein Registrierungsprofil für Apple-Geräte Registrierungsprogramme (DEP) dar, das für die iOS-Konfiguration spezifisch ist. Dieser Profiltyp muss Apple DEP-Seriennummern zugewiesen werden, bevor die entsprechenden Geräte über DEP registriert werden können.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79d2c041dfe3794afdb233a36d3a1f3d66ab1d04
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163931"
---
# <a name="depiosenrollmentprofile-resource-type"></a>depIOSEnrollmentProfile-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die DepIOSEnrollmentProfile-Ressource stellt ein Registrierungsprofil für Apple-Geräte Registrierungsprogramme (DEP) dar, das für die iOS-Konfiguration spezifisch ist. Dieser Profiltyp muss Apple DEP-Seriennummern zugewiesen werden, bevor die entsprechenden Geräte über DEP registriert werden können.


Erbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DepIOSEnrollmentProfiles aufListen](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekte.|
|[DepIOSEnrollmentProfile abrufen](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Lesen von Eigenschaften und Beziehungen des [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.|
|[DepIOSEnrollmentProfile erstellen](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Erstellen eines neuen [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.|
|[DepIOSEnrollmentProfile löschen](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|Keine|Löscht eine [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).|
|[DepIOSEnrollmentProfile aktualisieren](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Aktualisieren der Eigenschaften eines [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Die GUID für das von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Objekt.|
|displayName|Zeichenfolge|Name des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils|
|description|Zeichenfolge|Beschreibung des von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbten Profils|
|requiresUserAuthentication|Boolescher Wert|Gibt an, ob für das Profil eine von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Benutzerauthentifizierung erforderlich ist.|
|configurationEndpointUrl|Zeichenfolge|Konfigurations Endpunkt-URL für die von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbte Registrierung|
|enableAuthenticationViaCompanyPortal|Boolescher Wert|Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll. Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolescher Wert|Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten erforderlich ist, der von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) geerbt wurde.|
|isDefault|Boolescher Wert|Gibt an, ob dies das Standardprofil ist, das von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.|
|supervisedModeEnabled|Boolescher Wert|Überwachter Modus, true, um zu aktivieren, andernfalls false. Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter. Geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|Zeichenfolge|Von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbte Support Abteilungsinformationen|
|passCodeDisabled|Boolescher Wert|Gibt an, ob der Bereich "Passcode" deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Boolescher Wert|Gibt an, ob das Profil obligatorisch von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.|
|locationDisabled|Boolescher Wert|Gibt an, ob der speicherortdienst-Setup Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Zeichenfolge|Von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbte Support Telefonnummer|
|profileRemovalDisabled|Boolescher Wert|Gibt an, ob die Profil Entfernungs Option deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Boolescher Wert|Gibt an, ob der wiederHerstellungs-Setup Bereich von [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) geerbt wurde.|
|appleIdDisabled|Boolescher Wert|Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolescher Wert|Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolescher Wert|Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Boolescher Wert|Gibt an, ob der Apple Pay Setup-Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|zoomDisabled|Boolescher Wert|Gibt an, ob der Zoom-Installationsbereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Boolescher Wert|Gibt an, ob Siri-Setup Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolescher Wert|Gibt an, ob der Diagnose-Setup-Bereich deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Boolescher Wert|Gibt an, ob displaytone-Setupbildschirm deaktiviert ist geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Boolescher Wert|Gibt an, ob der Datenschutz Bildschirm deaktiviert ist, geerbt von [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Gibt den iTunes-paarungsmodus an. Mögliche Werte sind: `disallow`, `allow` und `requiresCertificate`.|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) -Sammlung|Verwaltungszertifikate für Apple Configurator|
|restoreFromAndroidDisabled|Boolescher Wert|Gibt an, ob die Wiederherstellung von Android deaktiviert ist.|
|awaitDeviceConfiguredConfirmation|Boolescher Wert|Gibt an, ob das Gerät auf die konfigurierte Bestätigung warten muss.|
|sharedIPadMaximumUserCount|Int32|Dies gibt die maximale Anzahl von Benutzern an, die ein freigegebenes iPad verwenden können. Gilt nur für den freigegebenen iPad-Modus.|
|Enablesharedipad wurden|Boolescher Wert|Dieser Wert gibt an, ob das Gerät in einen Modus eingeschrieben werden soll, der mehrere Benutzerszenarien ermöglicht. Gilt nur für freigegebene iPads.|
|companyPortalVppTokenId|Zeichenfolge|Wenn festgelegt, gibt das VSS-Token an, das zum Bereitstellen des Unternehmensportals mit der Geräte Lizenzierung verwendet werden soll. ' enableAuthenticationViaCompanyPortal ' muss festgelegt werden, damit diese Eigenschaft festgelegt wird.|
|enableSingleAppEnrollmentMode|Boolescher Wert|Weist das Gerät an, den Einzel APP-Modus zu aktivieren und die APP-Sperre während der Registrierung anzuwenden. Der Standardwert ist false. "enableAuthenticationViaCompanyPortal" und "companyPortalVppTokenId" müssen festgelegt werden, damit diese Eigenschaft festgelegt wird.|
|homeButtonScreenDisabled|Boolescher Wert|Gibt an, ob der Bildschirm für die Home-Schaltfläche deaktiviert ist|
|iMessageAndFaceTimeScreenDisabled|Boolescher Wert|Gibt an, ob iMessage-und FaceTime-Bildschirm deaktiviert sind.|
|onBoardingScreenDisabled|Boolescher Wert|Gibt an, ob der Bildschirm Onboarding Setup deaktiviert ist.|
|screenTimeScreenDisabled|Boolescher Wert|Gibt an, ob die Installation des Bildschirm Timeouts deaktiviert ist.|
|simSetupScreenDisabled|Boolescher Wert|Gibt an, ob der SIMSetup-Bildschirm deaktiviert ist.|
|softwareUpdateScreenDisabled|Boolescher Wert|Gibt an, ob der Bildschirm obligatorische Softwareaktualisierung deaktiviert ist.|
|watchMigrationScreenDisabled|Boolescher Wert|Gibt an, ob der Bildschirm für die Überwachung der Migration deaktiviert ist.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




