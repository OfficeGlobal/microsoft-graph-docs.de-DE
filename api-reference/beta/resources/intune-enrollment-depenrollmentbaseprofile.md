---
title: depEnrollmentBaseProfile-Ressourcentyp
description: Die DepEnrollmentBaseProfile-Ressource stellt ein Registrierungsprofil für das Apple-Geräte Registrierungsprogramm (DEP) dar. Dieser Profiltyp muss Apple DEP-Seriennummern zugewiesen werden, bevor die entsprechenden Geräte über DEP registriert werden können.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5ad27470bb09313084feadcf468d83e58964532
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143106"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>depEnrollmentBaseProfile-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die DepEnrollmentBaseProfile-Ressource stellt ein Registrierungsprofil für das Apple-Geräte Registrierungsprogramm (DEP) dar. Dieser Profiltyp muss Apple DEP-Seriennummern zugewiesen werden, bevor die entsprechenden Geräte über DEP registriert werden können.


Erbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DepEnrollmentBaseProfiles aufListen](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekte.|
|[DepEnrollmentBaseProfile abrufen](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Lesen von Eigenschaften und Beziehungen des [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekts.|

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
|isDefault|Boolescher Wert|Gibt an, ob dies das Standardprofil ist.|
|supervisedModeEnabled|Boolescher Wert|Überwachter Modus, true, um zu aktivieren, andernfalls false. Weitere https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Informationen finden Sie unter.|
|supportDepartment|Zeichenfolge|Informationen zur Support Abteilung|
|passCodeDisabled|Boolescher Wert|Gibt an, ob der Bereich "Passcode" deaktiviert ist.|
|isMandatory|Boolescher Wert|Gibt an, ob das Profil obligatorisch ist.|
|locationDisabled|Boolescher Wert|Gibt an, ob der Standortdienst-Setup Bereich deaktiviert ist.|
|supportPhoneNumber|Zeichenfolge|Support-Telefonnummer|
|profileRemovalDisabled|Boolescher Wert|Gibt an, ob die Profil Entfernungs Option deaktiviert ist.|
|restoreBlocked|Boolescher Wert|Gibt an, ob der wiederHerstellungs-Setup Bereich blockiert ist|
|appleIdDisabled|Boolescher Wert|Gibt an, ob der Apple ID-Setup Bereich deaktiviert ist.|
|termsAndConditionsDisabled|Boolescher Wert|Gibt an, ob der Setup Bereich "Bedingungen" deaktiviert ist.|
|touchIdDisabled|Boolescher Wert|Gibt an, ob der Bereich "Touch ID-Setup" deaktiviert ist.|
|applePayDisabled|Boolescher Wert|Gibt an, ob der Apple Pay-Setup Bereich deaktiviert ist.|
|zoomDisabled|Boolescher Wert|Gibt an, ob der Zoom-Setup Bereich deaktiviert ist.|
|siriDisabled|Boolescher Wert|Gibt an, ob der Siri-Setup Bereich deaktiviert ist.|
|diagnosticsDisabled|Boolescher Wert|Gibt an, ob der Diagnose-Setup Bereich deaktiviert ist.|
|displayToneSetupDisabled|Boolescher Wert|Gibt an, ob der displaytone-Setupbildschirm deaktiviert ist.|
|privacyPaneDisabled|Boolescher Wert|Gibt an, ob der Datenschutz Bildschirm deaktiviert ist.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
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
  "privacyPaneDisabled": true
}
```




