---
title: Ressourcentyp depEnrollmentBaseProfile
description: Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b820959e5515a575e4f074a2762794a15e7f5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423755"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>Ressourcentyp depEnrollmentBaseProfile

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können


Erbt vom [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Auflistung|Listeneigenschaften und Beziehungen der [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekte.|
|[Abrufen von depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Lesen Sie Eigenschaften und Beziehungen des [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Zeichenfolge|Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Zeichenfolge|Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert|
|configurationEndpointUrl|Zeichenfolge|Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration|
|enableAuthenticationViaCompanyPortal|Boolean|Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal. Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erforderlich ist|
|isDefault|Boolean|Gibt an, ob dies das Standardprofil ist|
|supervisedModeEnabled|Boolean|Überwachten Modus aktivieren, False andernfalls True. Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.|
|supportDepartment|Zeichenfolge|Abteilung Supportinformationen|
|passCodeDisabled|Boolean|Gibt an, ob Kennung Setup Bereich deaktiviert ist|
|isMandatory|Boolean|Gibt an, ob das Profil zwingend erforderlich ist.|
|locationDisabled|Boolean|Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist|
|supportPhoneNumber|Zeichenfolge|Support-Telefonnummer|
|profileRemovalDisabled|Boolean|Gibt an, ob die Option Profil entfernen deaktiviert ist|
|restoreBlocked|Boolean|Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist|
|appleIdDisabled|Boolean|Gibt an, ob Apple Id Setup Bereich deaktiviert ist|
|termsAndConditionsDisabled|Boolean|Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist|
|touchIdDisabled|Boolean|Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist|
|applePayDisabled|Boolean|Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist|
|zoomDisabled|Boolean|Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist|
|siriDisabled|Boolean|Gibt an, ob Siri Setup Bereich deaktiviert ist|
|diagnosticsDisabled|Boolean|Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist|
|displayToneSetupDisabled|Boolean|Gibt an, ob Displaytone Setupbildschirm deaktiviert ist|
|privacyPaneDisabled|Boolean|Gibt an, ob Privacy Bildschirm deaktiviert ist|

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




