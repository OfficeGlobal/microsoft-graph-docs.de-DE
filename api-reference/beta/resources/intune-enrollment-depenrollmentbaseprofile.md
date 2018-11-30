---
title: Ressourcentyp depEnrollmentBaseProfile
description: Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können
ms.openlocfilehash: 172e0f0d4ed9b23f8c5a3d5226e24e4ac63b0527
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064926"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>Ressourcentyp depEnrollmentBaseProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|profileRemovalDisabled|Boolesch|Gibt an, ob die Option Profil entfernen deaktiviert ist|
|restoreBlocked|Boolesch|Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist|
|appleIdDisabled|Boolesch|Gibt an, ob Apple Id Setup Bereich deaktiviert ist|
|termsAndConditionsDisabled|Boolesch|Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist|
|touchIdDisabled|Boolesch|Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist|
|applePayDisabled|Boolesch|Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist|
|zoomDisabled|Boolesch|Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist|
|siriDisabled|Boolesch|Gibt an, ob Siri Setup Bereich deaktiviert ist|
|diagnosticsDisabled|Boolesch|Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist|

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
  "diagnosticsDisabled": true
}
```





