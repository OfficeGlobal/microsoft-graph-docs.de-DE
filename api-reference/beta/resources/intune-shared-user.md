---
title: user-Ressourcentyp
description: Stellt ein user-Objekt von Azure Active Directory dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f7c49f6016c0cd91d80278282c937ad9ad9a0ab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422481"
---
# <a name="user-resource-type"></a>user-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Stellt ein user-Objekt von Azure Active Directory dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste Benutzer](../api/intune-shared-user-list.md) -Objekte.|[user](../resources/intune-shared-user.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.|
|[Abrufen von Benutzer](../api/intune-shared-user-get.md) -Objekt.|[user](../resources/intune-shared-user.md)|Lesen von Eigenschaften und Beziehungen des [user](../resources/intune-shared-user.md)-Objekts.|
|[Create User](../api/intune-shared-user-create.md) -Objekt.|[user](../resources/intune-shared-user.md)|Dient zum Erstellen eines neuen [user](../resources/intune-shared-user.md)-Objekts.|
|[Benutzer löschen](../api/intune-shared-user-delete.md).|Keine|Löscht einen [user](../resources/intune-shared-user.md).|
|[Update](../api/intune-shared-user-update.md) -Benutzerobjekt.|[user](../resources/intune-shared-user.md)|Aktualisieren der Eigenschaften eines [user](../resources/intune-shared-user.md)-Objekts.|
|**deviceManagement**|
|[GetLoggedOnManagedDevices-Funktion](../api/intune-shared-user-getloggedonmanageddevices.md)|[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung|Noch nicht dokumentiert|
|[removeAllDevicesFromManagement-Aktion](../api/intune-shared-user-removealldevicesfrommanagement.md)|Keine|Die Verwaltung aller Geräte für diesen Benutzer einstellen.|
|**Mobile Verwaltung (MAM)**|
|[getManagedAppDiagnosticStatuses-Funktion](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)-Sammlung|Ruft den Status der Diagnoseüberprüfung für einen bestimmten Benutzer ab.|
|[getManagedAppPolicies-Funktion](../api/intune-shared-user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung|Ruft App-Einschränkungen für einen bestimmten Benutzer ab.|
|[WipeManagedAppRegistrationByDeviceTag Aktion](../api/intune-shared-user-wipemanagedappregistrationbydevicetag.md)|Keine|Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.|
|[wipeManagedAppRegistrationsByDeviceTag-Aktion](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|Keine|Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.|
|**Onboarding**|
|[ExportDeviceAndAppManagementData-Funktion](../api/intune-shared-user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md)|Noch nicht dokumentiert|
|[GetEffectiveDeviceEnrollmentConfigurations-Funktion](../api/intune-shared-user-geteffectivedeviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Noch nicht dokumentiert|
|**Problembehandlung**|
|[GetManagedDevicesWithAppFailures-Funktion](../api/intune-shared-user-getmanageddeviceswithappfailures.md)|Zeichenfolgenauflistung|Ruft die Liste der Geräte mit fehlerhaften apps.|


## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner des Benutzers|
|**Onboarding**|
|deviceEnrollmentLimit|Int32|Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann. Zulässige Werte sind 5 oder 1000.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**deviceManagement**|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung|Die mit dem Benutzer verknüpften verwalteten Geräte.|
|**Mobile Verwaltung (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)-Sammlung|Null oder mehr verwaltete App-Registrierungen, die dem Benutzer gehören.|
|**Onboarding**|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Abrufen der Registrierung Konfigurationen geplant, für den Benutzer|
|**Problembehandlung**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für diesen Benutzer.|
|mobileAppIntentAndStates|[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Auflistung|Die Liste der Problembehandlungsereignisse für diesen Benutzer.|
|mobileAppTroubleshootingEvents|[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Auflistung|Die Liste der mobilen app Problembehandlung Ereignisse für diesen Benutzer.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



