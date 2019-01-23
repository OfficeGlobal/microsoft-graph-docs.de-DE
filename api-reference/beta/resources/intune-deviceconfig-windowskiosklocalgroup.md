---
title: Ressourcentyp windowsKioskLocalGroup
description: Die Klasse verwendet, um eine lokale Gruppe für die Konfiguration Kiosk identifizieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1134b6a842b54dc49fcd15a92d21aef227b35182
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424630"
---
# <a name="windowskiosklocalgroup-resource-type"></a>Ressourcentyp windowsKioskLocalGroup

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Klasse verwendet, um eine lokale Gruppe für die Konfiguration Kiosk identifizieren


Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|groupName|Zeichenfolge|Der Name der lokalen Gruppe, die mit dieser Konfiguration Kiosk gesperrt wird|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```




