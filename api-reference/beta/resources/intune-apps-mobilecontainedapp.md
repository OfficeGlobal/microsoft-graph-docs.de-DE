---
title: Ressourcentyp mobileContainedApp
description: Eine abstrakte Klasse, die eine enthaltene-app in einem MobileApp fungiert als Paket darstellt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b81ee4ca194d1d01e3d834b3287f6b400e712a27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826285"
---
# <a name="mobilecontainedapp-resource-type"></a>Ressourcentyp mobileContainedApp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Klasse, die eine enthaltene-app in einem MobileApp fungiert als Paket darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Auflistung|Listeneigenschaften und Beziehungen der [MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Objekte.|
|[Abrufen von mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Lesen Sie Eigenschaften und Beziehungen des [MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|

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





