---
title: Ressourcentyp userAppInstallStatus
description: Enthält Eigenschaften für den Installationsstatus für einen Benutzer.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1e1369e35af2343bebd609c760075a830649a1f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399892"
---
# <a name="userappinstallstatus-resource-type"></a>Ressourcentyp userAppInstallStatus

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Enthält Eigenschaften für den Installationsstatus für einen Benutzer.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Auflistung|Listeneigenschaften und Beziehungen der [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekte.|
|[Abrufen von userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Lesen Sie Eigenschaften und Beziehungen des [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|
|[Erstellen von userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Erstellen eines neuen [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|
|[UserAppInstallStatus löschen](../api/intune-apps-userappinstallstatus-delete.md)|Keine|Löscht eine [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[UserAppInstallStatus aktualisieren](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Aktualisieren Sie die Eigenschaften eines [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userName|String|Name des Benutzers|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname.|
|installedDeviceCount|Int32|Anzahl der installierten Geräte|
|failedDeviceCount|Int32|Anzahl der fehlgeschlagenen Geräte|
|notInstalledDeviceCount|Int32|Anzahl der nicht installierten Geräte|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|App|[mobileApp](../resources/intune-apps-mobileapp.md)|Den Navigationslink an die mobile app.|
|deviceStatuses|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Auflistung|Der Installationsstatus der app auf Geräten.|

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




