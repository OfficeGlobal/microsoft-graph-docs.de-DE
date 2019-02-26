---
title: windowsUniversalAppXContainedApp-Ressourcentyp
description: Eine Klasse, die eine enthaltene App einer WindowsUniversalAppX-APP darstellt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68c7c8a18e3d22b983a232859f5d56d73a79cc87
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157925"
---
# <a name="windowsuniversalappxcontainedapp-resource-type"></a>windowsUniversalAppXContainedApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine Klasse, die eine enthaltene App einer WindowsUniversalAppX-APP darstellt.


Erbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsUniversalAppXContainedApps aufListen](../api/intune-apps-windowsuniversalappxcontainedapp-list.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekte.|
|[WindowsUniversalAppXContainedApp abrufen](../api/intune-apps-windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Lesen von Eigenschaften und Beziehungen des [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.|
|[WindowsUniversalAppXContainedApp erstellen](../api/intune-apps-windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Erstellen eines neuen [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.|
|[WindowsUniversalAppXContainedApp löschen](../api/intune-apps-windowsuniversalappxcontainedapp-delete.md)|Keine|Löscht eine [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).|
|[WindowsUniversalAppXContainedApp aktualisieren](../api/intune-apps-windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|Aktualisieren der Eigenschaften eines [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|Zeichenfolge|Die APP-Benutzermodell-ID der enthaltenen App einer WindowsUniversalAppX-app.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppXContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```




