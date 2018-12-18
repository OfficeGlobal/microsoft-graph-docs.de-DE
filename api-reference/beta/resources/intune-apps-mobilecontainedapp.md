---
title: Ressourcentyp mobileContainedApp
description: Eine abstrakte Klasse, die eine enthaltene-app in einem MobileApp fungiert als Paket darstellt.
author: tfitzmac
ms.openlocfilehash: 314225c46247bd122c825f0f883378513445ce0a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340796"
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





