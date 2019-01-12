---
title: Ressourcentyp iosBookmark
description: iOS-URL-Textmarke
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbf39a2eee5064b7d3ddfa474b1f70758d4c7047
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938174"
---
# <a name="iosbookmark-resource-type"></a>Ressourcentyp iosBookmark

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

iOS-URL-Textmarke
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|url|Zeichenfolge|URL für den Zugriff auf zulässige|
|bookmarkFolder|Zeichenfolge|Der Ordner, in dem die Textmarke in Safari hinzugefügt werden soll|
|displayName|Zeichenfolge|Der Anzeigename der Textmarke|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```





