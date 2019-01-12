---
title: Ressourcentyp depEnrollmentBaseProfile
description: Die Ressource DepEnrollmentBaseProfile stellt ein Apple Gerät Registrierung Programm (DEP) Registrierung-Profil. Dieser Typ des Profils muss Apple DEP Seriennummer zugewiesen werden, bevor die entsprechende Geräte über Datenausführungsverhinderung registrieren können
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e1383048b08a309ea0ecf60eb1ad07c2636e7e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937670"
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
|id|Zeichenfolge|Die GUID für das Objekt Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Zeichenfolge|Name des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Zeichenfolge|Beschreibung des Profils Inherited aus [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolescher Wert|Gibt an, ob das Profil Benutzerauthentifizierung Inherited aus [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) erfordert|
|configurationEndpointUrl|Zeichenfolge|Endpunkt-Url für die Registrierung geerbt von [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) zu verwendende Konfiguration|
|enableAuthenticationViaCompanyPortal|Boolescher Wert|Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal. Geerbt von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolescher Wert|Gibt an, ob dies das Standardprofil ist|
|supervisedModeEnabled|Boolescher Wert|Überwachten Modus aktivieren, False andernfalls True. Finden Sie unter https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune Weitere Informationen.|
|supportDepartment|Zeichenfolge|Abteilung Supportinformationen|
|passCodeDisabled|Boolescher Wert|Gibt an, ob Kennung Setup Bereich deaktiviert ist|
|isMandatory|Boolescher Wert|Gibt an, ob das Profil zwingend erforderlich ist.|
|locationDisabled|Boolescher Wert|Gibt an, ob im Bereich Speicherort Service-Setup deaktiviert ist|
|supportPhoneNumber|Zeichenfolge|Support-Telefonnummer|
|profileRemovalDisabled|Boolescher Wert|Gibt an, ob die Option Profil entfernen deaktiviert ist|
|restoreBlocked|Boolescher Wert|Gibt an, ob die Wiederherstellung Setup Bereich gesperrt ist|
|appleIdDisabled|Boolescher Wert|Gibt an, ob Apple Id Setup Bereich deaktiviert ist|
|termsAndConditionsDisabled|Boolescher Wert|Gibt an, ob im Bereich 'Geschäftsbedingungen'-Setup deaktiviert ist|
|touchIdDisabled|Boolescher Wert|Gibt an, ob im Bereich Touch-Id-Setup deaktiviert ist|
|applePayDisabled|Boolescher Wert|Gibt an, ob Apple Lohn Setup Bereich deaktiviert ist|
|zoomDisabled|Boolescher Wert|Gibt an, ob der Bereich der Zoom-Setup deaktiviert ist|
|siriDisabled|Boolescher Wert|Gibt an, ob Siri Setup Bereich deaktiviert ist|
|diagnosticsDisabled|Boolescher Wert|Gibt an, ob der Bereich der Diagnose-Setup deaktiviert ist|

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





