---
title: Ressourcentyp mobileContainedApp
description: Eine abstrakte Klasse, die eine enthaltene-app in einem MobileApp fungiert als Paket darstellt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5d4ed392d681d97478cb1baf5ff6f854cb74011
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425666"
---
# <a name="mobilecontainedapp-resource-type"></a>Ressourcentyp mobileContainedApp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Eine abstrakte Klasse, die eine enthaltene-app in einem MobileApp fungiert als Paket darstellt.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Auflistung|Listeneigenschaften und Beziehungen der [MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Objekte.|
|[Abrufen von mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Lesen Sie Eigenschaften und Beziehungen des [MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Objekts.|

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




