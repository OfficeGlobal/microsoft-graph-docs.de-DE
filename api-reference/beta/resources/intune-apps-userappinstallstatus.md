---
title: userAppInstallStatus-Ressourcentyp
description: Enthält Eigenschaften für den Installationsstatus für einen Benutzer.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4778728fbec389b276e5098ffa859f13ccb6a9e4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143960"
---
# <a name="userappinstallstatus-resource-type"></a>userAppInstallStatus-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für den Installationsstatus für einen Benutzer.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[UserAppInstallStatuses aufListen](../api/intune-apps-userappinstallstatus-list.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekte.|
|[UserAppInstallStatus abrufen](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Lesen von Eigenschaften und Beziehungen des [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|
|[UserAppInstallStatus erstellen](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Erstellen eines neuen [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|
|[UserAppInstallStatus löschen](../api/intune-apps-userappinstallstatus-delete.md)|Keine|Löscht eine [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[UserAppInstallStatus aktualisieren](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Aktualisieren der Eigenschaften eines [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userName|String|Name des Benutzers|
|userPrincipalName|Zeichenfolge|Benutzerprinzipal Name.|
|installedDeviceCount|Int32|Anzahl der installierten Geräte|
|failedDeviceCount|Int32|Anzahl der fehlgeschlagenen Geräte|
|notInstalledDeviceCount|Int32|Anzahl der nicht installierten Geräte|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|App|[mobileApp](../resources/intune-apps-mobileapp.md)|Der Navigationslink zur mobilen App.|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Sammlung|Der Installationsstatus der APP auf Geräten.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```




