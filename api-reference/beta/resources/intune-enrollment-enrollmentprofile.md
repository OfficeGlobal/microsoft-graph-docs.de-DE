---
title: Ressourcentyp enrollmentProfile
description: Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren. Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a7ce4aac1e22610d539419dd6a63d124616b83f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396840"
---
# <a name="enrollmentprofile-resource-type"></a>Ressourcentyp enrollmentProfile

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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
|requiresUserAuthentication|Boolean|Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert|
|configurationEndpointUrl|Zeichenfolge|Endpunkt-Url für die Registrierung zu verwendende Konfiguration|
|enableAuthenticationViaCompanyPortal|Boolean|Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten erforderlich ist|

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
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




