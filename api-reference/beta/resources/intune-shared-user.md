---
title: user-Ressourcentyp
description: Stellt ein user-Objekt von Azure Active Directory dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: daa6f7a4802341347f364040504368dc96d75e33
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163371"
---
# <a name="user-resource-type"></a>user-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt ein user-Objekt von Azure Active Directory dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|AufListen von [Users](../api/intune-shared-user-list.md) -Objekten.|[user](../resources/intune-shared-user.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.|
|[Benutzerobjekt abrufen](../api/intune-shared-user-get.md) .|[user](../resources/intune-shared-user.md)|Lesen von Eigenschaften und Beziehungen des [user](../resources/intune-shared-user.md)-Objekts.|
|[Benutzerobjekt erstellen](../api/intune-shared-user-create.md) .|[user](../resources/intune-shared-user.md)|Dient zum Erstellen eines neuen [user](../resources/intune-shared-user.md)-Objekts.|
|[Benutzer löschen](../api/intune-shared-user-delete.md).|Keine|Löscht einen [user](../resources/intune-shared-user.md).|
|[Benutzerobjekt aktualisieren](../api/intune-shared-user-update.md) .|[user](../resources/intune-shared-user.md)|Aktualisieren der Eigenschaften eines [user](../resources/intune-shared-user.md)-Objekts.|
|**deviceManagement**|
|[getLoggedOnManagedDevices-Funktion](../api/intune-shared-user-getloggedonmanageddevices.md)|[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung|Noch nicht dokumentiert|
|[removeAllDevicesFromManagement-Aktion](../api/intune-shared-user-removealldevicesfrommanagement.md)|Keine|Die Verwaltung aller Geräte für diesen Benutzer einstellen.|
|**Mobile Anwendungsverwaltung (MAM)**|
|[getManagedAppDiagnosticStatuses-Funktion](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)-Sammlung|Ruft den Status der Diagnoseüberprüfung für einen bestimmten Benutzer ab.|
|[getManagedAppPolicies-Funktion](../api/intune-shared-user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung|Ruft App-Einschränkungen für einen bestimmten Benutzer ab.|
|[wipeManagedAppRegistrationByDeviceTag-Aktion](../api/intune-shared-user-wipemanagedappregistrationbydevicetag.md)|Keine|Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.|
|[wipeManagedAppRegistrationsByDeviceTag-Aktion](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|Keine|Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.|
|**Onboarding**|
|[exportDeviceAndAppManagementData-Funktion](../api/intune-shared-user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md)|Noch nicht dokumentiert|
|[getEffectiveDeviceEnrollmentConfigurations-Funktion](../api/intune-shared-user-geteffectivedeviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Noch nicht dokumentiert|
|**Problembehandlung**|
|[getManagedDevicesWithAppFailures-Funktion](../api/intune-shared-user-getmanageddeviceswithappfailures.md)|String collection|Ruft die Liste der Geräte mit fehlgeschlagenen apps ab.|


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
|**Mobile Anwendungsverwaltung (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)-Sammlung|Null oder mehr verwaltete App-Registrierungen, die dem Benutzer gehören.|
|**Onboarding**|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Abrufen von Registrierungs Konfigurationen für den Benutzer|
|**Problembehandlung**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für diesen Benutzer.|
|mobileAppIntentAndStates|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Sammlung|Die Liste der Problembehandlungsereignisse für diesen Benutzer.|
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Sammlung|Die Liste der Problembehandlungsereignisse für Mobile Apps für diesen Benutzer.|

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



