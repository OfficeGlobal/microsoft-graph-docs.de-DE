---
title: windowsPrivacyDataAccessControlItem-Ressourcentyp
description: Angeben der Zugriffs Steuerungsebene pro Datenschutzkategorie
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9589eab792620a2b534473ba9544d97c93ae8910
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174060"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>windowsPrivacyDataAccessControlItem-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Angeben der Zugriffs Steuerungsebene pro Datenschutzkategorie

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsPrivacyDataAccessControlItems aufListen](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekte.|
|[WindowsPrivacyDataAccessControlItem abrufen](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Lesen von Eigenschaften und Beziehungen des [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.|
|[WindowsPrivacyDataAccessControlItem erstellen](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Erstellen eines neuen [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.|
|[WindowsPrivacyDataAccessControlItem löschen](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|Keine|Löscht eine [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).|
|[WindowsPrivacyDataAccessControlItem aktualisieren](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Aktualisieren der Eigenschaften eines [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Der Schlüssel von WindowsPrivacyDataAccessControlItem.|
|Access Level|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|Dies gibt eine Zugriffsebene für die Datenschutzkategorie an, der die angegebene Anwendung zugewiesen wird. Mögliche Werte: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|Dies gibt eine Datenschutzkategorie an, auf die die spezifische Zugriffssteuerung angewendet werden soll. Mögliche Werte sind: `notConfigured`, `accountInfo`, `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `email` `location` `messaging` `microphone` `motion` `notifications` `phone`,,,,,,,, `radios`,, `trustedDevices` ,,,,,, `tasks` `syncWithDevices` `diagnosticsInfo` .|
|appPackageFamilyName|Zeichenfolge|Der Name der Paketfamilie einer Windows-app. Wenn diese Einstellung festgelegt ist, gilt die Zugriffsebene für die angegebene Anwendung.|
|appDisplayName|Zeichenfolge|Der Name der Paketfamilie einer Windows-app. Wenn diese Einstellung festgelegt ist, gilt die Zugriffsebene für die angegebene Anwendung.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```




