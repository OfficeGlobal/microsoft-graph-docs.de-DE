---
title: Ressourcentyp windows10AssociatedApps
description: Definition der Windows-10-Anwendung verknüpft ist.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5dd5b664bde2970caa4b09c027592684b9ecd5e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425918"
---
# <a name="windows10associatedapps-resource-type"></a>Ressourcentyp windows10AssociatedApps

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Definition der Windows-10-Anwendung verknüpft ist.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|der appType|[windows10AppType](../resources/intune-deviceconfig-windows10apptype.md)|Anwendungstyp. Mögliche Werte sind: `desktop` und `universal`.|
|Bezeichner|Zeichenfolge|Bezeichner.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```




