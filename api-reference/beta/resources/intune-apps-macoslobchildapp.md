---
title: Ressourcentyp macOSLobChildApp
description: Enthält Eigenschaften, die die Mac OS LOB-App in einem Paket bundle
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43f207bb2cebccdd01c791694674c6fbf96b631f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954232"
---
# <a name="macoslobchildapp-resource-type"></a>Ressourcentyp macOSLobChildApp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften, die die Mac OS LOB-App in einem Paket bundle
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|bundleId|Zeichenfolge|Identitätsname|
|buildNumber|Zeichenfolge|Die Buildnummer der Mac OS-Zeile des Business (LoB) app.|
|versionNumber|Zeichenfolge|Die Versionsnummer der Mac OS-Zeile des Business (LoB) app.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





