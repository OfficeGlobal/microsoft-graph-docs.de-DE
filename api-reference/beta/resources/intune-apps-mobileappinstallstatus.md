---
title: Ressourcentyp mobileAppInstallStatus
description: Enthält Eigenschaften für den Installationsstatus von einer mobilen app bei einem Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cac5c94f0669f784bf4cdd020448e40799d53915
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982610"
---
# <a name="mobileappinstallstatus-resource-type"></a>Ressourcentyp mobileAppInstallStatus

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für den Installationsstatus von einer mobilen app bei einem Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Auflistung|Listeneigenschaften und Beziehungen der [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekte.|
|[Abrufen von mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Lesen Sie Eigenschaften und Beziehungen des [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.|
|[Erstellen von mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Erstellen eines neuen [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.|
|[MobileAppInstallStatus löschen](../api/intune-apps-mobileappinstallstatus-delete.md)|Keine|Löscht eine [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).|
|[MobileAppInstallStatus aktualisieren](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Aktualisieren Sie die Eigenschaften eines [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|deviceName|Zeichenfolge|Gerätename|
|deviceId|Zeichenfolge|Geräte-ID|
|lastSyncDateTime|DateTimeOffset|Letzte Synchronisierung Datum-Zeit|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-shared-resultantappstate.md)|Der Installationsstatus der app. Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.|
|installState|[resultantAppState](../resources/intune-shared-resultantappstate.md)|Der Installationsstatus der app. Mögliche Werte sind: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown` und `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Die Details der Installation Zustand der app. Mögliche Werte: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|errorCode|Int32|Der Fehler im code für die Installation oder Deinstallieren von Fehlern.|
|osVersion|Zeichenfolge|Version des Betriebssystems|
|osDescription|String|OS Beschreibung|
|userName|Zeichenfolge|Name des Aufnahmegeräts Benutzer|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname|
|displayVersion|Zeichenfolge|Menschen lesbare Version der Anwendung|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|App|[mobileApp](../resources/intune-apps-mobileapp.md)|Den Navigationslink an die mobile app.|

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





