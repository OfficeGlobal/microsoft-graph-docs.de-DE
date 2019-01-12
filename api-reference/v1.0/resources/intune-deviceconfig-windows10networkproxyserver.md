---
title: windows10NetworkProxyServer-Ressourcentyp
description: Netzwerk-Proxyserverrichtlinie.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4e9f727916f055fe197f98b07625b00406e16e83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921101"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Netzwerk-Proxyserverrichtlinie.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|address|String|Adresse des Proxyservers. Geben Sie eine Adresse im Format <server>\[":"<port>\] an.|
|exceptions|String-Sammlung|Adressen, die den Proxyserver nicht verwenden sollten. Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.|
|useForLocalAddresses|Boolean|Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



