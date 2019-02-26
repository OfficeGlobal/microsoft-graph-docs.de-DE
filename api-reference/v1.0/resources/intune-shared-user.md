---
title: user-Ressourcentyp
description: Stellt ein user-Objekt von Azure Active Directory dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7a6c87b5c073e00b660db807ff38c454c302d94
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253407"
---
# <a name="user-resource-type"></a>user-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt ein user-Objekt von Azure Active Directory dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|AufListen von [Users](../api/intune-shared-user-list.md) -Objekten.|[user](../resources/intune-shared-user.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.|
|[Benutzerobjekt abrufen](../api/intune-shared-user-get.md) .|[Benutzersammlung](../resources/intune-shared-user.md)|Lesen von Eigenschaften und Beziehungen des [user](../resources/intune-shared-user.md)-Objekts.|
|[Benutzerobjekt erstellen](../api/intune-shared-user-create.md) .|[Benutzersammlung](../resources/intune-shared-user.md)|Dient zum Erstellen eines neuen [user](../resources/intune-shared-user.md)-Objekts.|
|[Benutzer löschen](../api/intune-shared-user-delete.md).|Keine|Löscht einen [user](../resources/intune-shared-user.md).|
|[Benutzerobjekt aktualisieren](../api/intune-shared-user-update.md) .|[user](../resources/intune-shared-user.md)|Aktualisieren der Eigenschaften eines [user](../resources/intune-shared-user.md)-Objekts.|
|**deviceManagement**|
|[removeAllDevicesFromManagement-Aktion](../api/intune-shared-user-removealldevicesfrommanagement.md)|Keine|Die Verwaltung aller Geräte für diesen Benutzer einstellen.|
|**Mobile App Management (MAM)**|
|[getManagedAppDiagnosticStatuses-Funktion](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)-Sammlung|Ruft den Status der Diagnoseüberprüfung für einen bestimmten Benutzer ab.|
|[getManagedAppPolicies-Funktion](../api/intune-shared-user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung|Ruft App-Einschränkungen für einen bestimmten Benutzer ab.|
|[wipeManagedAppRegistrationsByDeviceTag-Aktion](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|Keine|Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.|

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
|**Mobile App Management (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)-Sammlung|Null oder mehr verwaltete App-Registrierungen, die dem Benutzer gehören.|
|**Problembehandlung**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für diesen Benutzer.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
--> 
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
