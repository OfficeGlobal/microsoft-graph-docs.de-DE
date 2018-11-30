---
title: Ressourcentyp windowsKioskAzureADGroup
description: Die Klasse verwendet, um eine Gruppe AzureAD für die Konfiguration Kiosk identifizieren
ms.openlocfilehash: 4853013c9c1e9d4c276ee5e2ba83cb8b36afd06c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058616"
---
# <a name="windowskioskazureadgroup-resource-type"></a>Ressourcentyp windowsKioskAzureADGroup

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Klasse verwendet, um eine Gruppe AzureAD für die Konfiguration Kiosk identifizieren

Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Der Anzeigename der Gruppe der AzureAD, die mit dieser Konfiguration Kiosk gesperrt wird|
|groupId|String|Die ID der AzureAD Gruppe, die mit dieser Konfiguration Kiosk gesperrt wird|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```





