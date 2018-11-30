---
title: Ressourcentyp iosWebContentFilterAutoFilter
description: Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung. Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.
ms.openlocfilehash: 04a221ac512ab3934702a2a9e3178ba23a2ac3ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063746"
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





