---
title: Ressourcentyp mobileAppIntentAndState
description: MobileApp beabsichtigt und Installationsstatus für ein bestimmtes Gerät.
author: tfitzmac
ms.openlocfilehash: 40ffbac3f86ccce3037a6585fa608dd4055bd428
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356056"
---
# <a name="mobileappintentandstate-resource-type"></a>Ressourcentyp mobileAppIntentAndState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

MobileApp beabsichtigt und Installationsstatus für ein bestimmtes Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste mobileAppIntentAndStates](../api/intune-troubleshooting-mobileappintentandstate-list.md)|[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Auflistung|Listeneigenschaften und Beziehungen der [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekte.|
|[Abrufen von mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Lesen Sie Eigenschaften und Beziehungen des [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.|
|[Erstellen von mobileAppIntentAndState](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Erstellen eines neuen [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.|
|[MobileAppIntentAndState löschen](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|Keines|Löscht eine [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).|
|[MobileAppIntentAndState aktualisieren](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Aktualisieren Sie die Eigenschaften eines [MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|UUID für das Objekt|
|managedDeviceIdentifier|String|Von Intune erstellter oder erfasster Gerätebezeichner|
|userId|String|Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.|
|mobileAppList|[MobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) -Auflistung|Die Liste der Nutzlast Intents und Status für den Mandanten.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppIntentAndState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "String (identifier)",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "String",
      "displayName": "String",
      "mobileAppIntent": "String",
      "displayVersion": "String",
      "installState": "String",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "String",
          "minimumOperatingSystemVersion": "String",
          "maximumOperatingSystemVersion": "String"
        }
      ]
    }
  ]
}
```





