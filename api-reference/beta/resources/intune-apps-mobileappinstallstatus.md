---
title: mobileAppInstallStatus-Ressourcentyp
description: Enthält Eigenschaften für den Installationsstatus einer mobilen App für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91dbe509db57153aa325ecf80c508d8ec47f69b7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162363"
---
# <a name="mobileappinstallstatus-resource-type"></a>mobileAppInstallStatus-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für den Installationsstatus einer mobilen App für ein Gerät.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileAppInstallStatuses aufListen](../api/intune-apps-mobileappinstallstatus-list.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekte.|
|[MobileAppInstallStatus abrufen](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.|
|[MobileAppInstallStatus erstellen](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Erstellen eines neuen [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.|
|[MobileAppInstallStatus löschen](../api/intune-apps-mobileappinstallstatus-delete.md)|Keine|Löscht eine [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).|
|[MobileAppInstallStatus aktualisieren](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Aktualisieren der Eigenschaften eines [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|deviceName|Zeichenfolge|Gerätename|
|deviceId|Zeichenfolge|Geräte-ID|
|lastSyncDateTime|DateTimeOffset|Datum der letzten Synchronisierung|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-shared-resultantappstate.md)|Der Installationsstatus der app. Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.|
|installState|[resultantAppState](../resources/intune-shared-resultantappstate.md)|Der Installationsstatus der app. Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Die Installationsstatus Details der app. Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|errorCode|Int32|Der Fehlercode für Installations-oder Deinstallationsfehler.|
|osVersion|Zeichenfolge|Betriebssystem Version|
|osDescription|String|Betriebssystem Beschreibung|
|userName|Zeichenfolge|Geräte Benutzer Name|
|userPrincipalName|String|Benutzerprinzipalname|
|Display Version|Zeichenfolge|Lesbare Version der Anwendung|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|App|[mobileApp](../resources/intune-apps-mobileapp.md)|Der Navigationslink zur mobilen App.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```




