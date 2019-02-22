---
title: mobileContainedApp-Ressourcentyp
description: Eine abstrakte Klasse, die eine enthaltene app in einem mobileApp darstellt, das als Paket fungiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3400349244e738644d4885b2265c5f7f4ceb84e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145199"
---
# <a name="mobilecontainedapp-resource-type"></a>mobileContainedApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine abstrakte Klasse, die eine enthaltene app in einem mobileApp darstellt, das als Paket fungiert.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileContainedApps aufListen](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Objekte.|
|[MobileContainedApp abrufen](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Lesen von Eigenschaften und Beziehungen des [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```




