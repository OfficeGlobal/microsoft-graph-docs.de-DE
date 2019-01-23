---
title: Ressourcentyp iosWebContentFilterAutoFilter
description: Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung. Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5be275b74e2675881b9d36b047e2017ef95adb2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401229"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>Ressourcentyp iosWebContentFilterAutoFilter

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung. Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.


Erbt vom [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|allowedUrls|Zeichenfolgenauflistung|Zusätzliche URLs für den Zugriff zulässig|
|blockedUrls|Zeichenfolgenauflistung|Zusätzliche URLs für den Zugriff blockiert|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```




