---
title: Ressourcentyp enrollmentProfile
description: Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren. Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b88745c060e71e32199a96b23f94fa0d3229d451
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935591"
---
# <a name="enrollmentprofile-resource-type"></a>Ressourcentyp enrollmentProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren. Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Auflistung|Listeneigenschaften und Beziehungen der [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekte.|
|[Abrufen von enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Lesen Sie Eigenschaften und Beziehungen des [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.|
|[Erstellen von enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Erstellen eines neuen [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.|
|[EnrollmentProfile löschen](../api/intune-enrollment-enrollmentprofile-delete.md)|Keine|Löscht eine [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).|
|[EnrollmentProfile aktualisieren](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Aktualisieren Sie die Eigenschaften eines [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.|
|[SetDefaultProfile Aktion](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|Keine|Noch nicht dokumentiert|
|[ExportMobileConfig-Funktion](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|Zeichenfolge|Exportiert die mobile Konfiguration|
|[UpdateDeviceProfileAssignment Aktion](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|displayName|Zeichenfolge|Name des Profils|
|description|Zeichenfolge|Beschreibung des Profils|
|requiresUserAuthentication|Boolescher Wert|Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert|
|configurationEndpointUrl|Zeichenfolge|Endpunkt-Url für die Registrierung zu verwendende Konfiguration|
|enableAuthenticationViaCompanyPortal|Boolescher Wert|Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true
}
```





