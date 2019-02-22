---
title: mobileAppIntentAndState-Ressourcentyp
description: MobileApp und Installationsstatus für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aff331007171f611ed96cadeee055f412f391e6b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163875"
---
# <a name="mobileappintentandstate-resource-type"></a>mobileAppIntentAndState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

MobileApp und Installationsstatus für ein bestimmtes Gerät.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileAppIntentAndStates aufListen](../api/intune-troubleshooting-mobileappintentandstate-list.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekte.|
|[MobileAppIntentAndState abrufen](../api/intune-troubleshooting-mobileappintentandstate-get.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.|
|[MobileAppIntentAndState erstellen](../api/intune-troubleshooting-mobileappintentandstate-create.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Erstellen eines neuen [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.|
|[MobileAppIntentAndState löschen](../api/intune-troubleshooting-mobileappintentandstate-delete.md)|Keine|Löscht eine [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).|
|[MobileAppIntentAndState aktualisieren](../api/intune-troubleshooting-mobileappintentandstate-update.md)|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Aktualisieren der Eigenschaften eines [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|UUID für das Objekt|
|managedDeviceIdentifier|Zeichenfolge|Von Intune erstellter oder erfasster Gerätebezeichner|
|userId|Zeichenfolge|Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.|
|mobileAppList|[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) -Sammlung|Die Liste der Payload-und Statusinformationen für den Mandanten.|

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




