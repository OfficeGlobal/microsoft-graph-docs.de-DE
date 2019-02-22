---
title: deviceConfigurationUserStateSummary-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 170b84d58d17bfbf8eea7d402c26b78019be3958
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163021"
---
# <a name="deviceconfigurationuserstatesummary-resource-type"></a>deviceConfigurationUserStateSummary-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceConfigurationUserStateSummary abrufen](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-get.md)|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekts.|
|[DeviceConfigurationUserStateSummary aktualisieren](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-update.md)|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|unknownUserCount|Int32|Anzahl Unbekannter Benutzer|
|notApplicableUserCount|Int32|Anzahl der nicht anwendbaren Benutzer|
|compliantUserCount|Int32|Anzahl der kompatiblen Benutzer|
|remediatedUserCount|Int32|Anzahl der beZahlten Benutzer|
|nonCompliantUserCount|Int32|Anzahl der nicht kompatiblen Benutzer|
|errorUserCount|Int32|Anzahl der Fehler Benutzer|
|conflictUserCount|Int32|Anzahl der Konflikt Benutzer|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "String (identifier)",
  "unknownUserCount": 1024,
  "notApplicableUserCount": 1024,
  "compliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "errorUserCount": 1024,
  "conflictUserCount": 1024
}
```




