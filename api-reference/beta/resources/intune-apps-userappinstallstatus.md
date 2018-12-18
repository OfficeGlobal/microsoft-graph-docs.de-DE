---
title: Ressourcentyp userAppInstallStatus
description: Enthält Eigenschaften für den Installationsstatus für einen Benutzer.
author: tfitzmac
ms.openlocfilehash: 024fff32aac2a268a2e0bbec81a6d46b31012a11
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302758"
---
# <a name="userappinstallstatus-resource-type"></a>Ressourcentyp userAppInstallStatus

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für den Installationsstatus für einen Benutzer.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Auflistung|Listeneigenschaften und Beziehungen der [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekte.|
|[Abrufen von userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Lesen Sie Eigenschaften und Beziehungen des [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|
|[Erstellen von userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Erstellen eines neuen [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|
|[UserAppInstallStatus löschen](../api/intune-apps-userappinstallstatus-delete.md)|Keines|Löscht eine [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[UserAppInstallStatus aktualisieren](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Aktualisieren Sie die Eigenschaften eines [UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|userName|String|Name des Benutzers|
|userPrincipalName|String|Benutzerprinzipalname.|
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





