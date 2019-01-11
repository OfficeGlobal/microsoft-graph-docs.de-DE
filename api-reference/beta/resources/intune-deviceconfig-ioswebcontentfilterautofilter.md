---
title: Ressourcentyp iosWebContentFilterAutoFilter
description: Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung. Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.
localization_priority: Normal
ms.openlocfilehash: 02576565ecf764d33312477531d6a76c61911cb6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868131"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>Ressourcentyp iosWebContentFilterAutoFilter

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung. Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.

Erbt vom [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|allowedUrls|Collection von Objekten des Typs „String“|Zusätzliche URLs für den Zugriff zulässig|
|blockedUrls|Collection von Objekten des Typs „String“|Zusätzliche URLs für den Zugriff blockiert|

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





