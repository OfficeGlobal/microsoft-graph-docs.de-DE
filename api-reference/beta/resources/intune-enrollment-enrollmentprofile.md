---
title: enrollmentProfile-Ressourcentyp
description: Die enrollmentProfile-Ressource stellt eine Auflistung von Konfigurationen dar, die vor der Registrierung bereitgestellt werden müssen, um die Anmeldung bestimmter Geräte zu ermöglichen, deren Identitäten bereits vorbereitt wurden. Diesem Profiltyp werden Pre-Staging-Geräte Identitäten zugewiesen, um die Konfigurationen des Profils bei der Registrierung des entsprechenden Geräts anzuwenden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d8947864611ac2c0d26256a5d739d41b86c383f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151177"
---
# <a name="enrollmentprofile-resource-type"></a>enrollmentProfile-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die enrollmentProfile-Ressource stellt eine Auflistung von Konfigurationen dar, die vor der Registrierung bereitgestellt werden müssen, um die Anmeldung bestimmter Geräte zu ermöglichen, deren Identitäten bereits vorbereitt wurden. Diesem Profiltyp werden Pre-Staging-Geräte Identitäten zugewiesen, um die Konfigurationen des Profils bei der Registrierung des entsprechenden Geräts anzuwenden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[EnrollmentProfiles aufListen](../api/intune-enrollment-enrollmentprofile-list.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekte.|
|[EnrollmentProfile abrufen](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Lesen von Eigenschaften und Beziehungen des [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.|
|[EnrollmentProfile erstellen](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Erstellen eines neuen [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.|
|[EnrollmentProfile löschen](../api/intune-enrollment-enrollmentprofile-delete.md)|Keine|Löscht eine [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).|
|[EnrollmentProfile aktualisieren](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Aktualisieren der Eigenschaften eines [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.|
|[setDefaultProfile-Aktion](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|Keine|Noch nicht dokumentiert|
|[exportMobileConfig-Funktion](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|Zeichenfolge|Exportiert die Mobile Konfiguration|
|[updateDeviceProfileAssignment-Aktion](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|displayName|Zeichenfolge|Name des Profils|
|description|Zeichenfolge|Beschreibung des Profils|
|requiresUserAuthentication|Boolescher Wert|Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert.|
|configurationEndpointUrl|Zeichenfolge|Konfigurations Endpunkt-URL für die Registrierung|
|enableAuthenticationViaCompanyPortal|Boolescher Wert|Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolescher Wert|Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten für registrierte Geräte erforderlich ist.|

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




