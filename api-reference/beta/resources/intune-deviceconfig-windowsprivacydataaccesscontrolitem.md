---
title: Ressourcentyp windowsPrivacyDataAccessControlItem
description: Geben Sie Control Zugriffsebene pro private Datenkategorie
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfce1de413168da685d7460f56a8ee98972c27e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952118"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>Ressourcentyp windowsPrivacyDataAccessControlItem

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Geben Sie Control Zugriffsebene pro private Datenkategorie
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsPrivacyDataAccessControlItems](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekte.|
|[Abrufen von windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.|
|[Erstellen von windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Erstellen eines neuen [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.|
|[WindowsPrivacyDataAccessControlItem löschen](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|Keines|Löscht eine [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).|
|[WindowsPrivacyDataAccessControlItem aktualisieren](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Aktualisieren Sie die Eigenschaften eines [WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Der Schlüssel des WindowsPrivacyDataAccessControlItem.|
|accessLevel|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|Dies bedeutet eine Zugriffsebene für die Kategorie private Daten an die für die angegebene Anwendung erhalten soll. Mögliche Werte: sind `notConfigured`, `forceAllow`, `forceDeny` und `userInControl`.|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|Dies bedeutet eine private Datenkategorie für die bestimmten Access Control gelten soll. Mögliche Werte sind: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices` .|
|appPackageFamilyName|Zeichenfolge|Die Paket-Produktfamilie Name einer Windows-App. Wenn festgelegt, gilt die Zugriffsebene für die angegebene Anwendung.|
|appDisplayName|Zeichenfolge|Die Paket-Produktfamilie Name einer Windows-App. Wenn festgelegt, gilt die Zugriffsebene für die angegebene Anwendung.|

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





