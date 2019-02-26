---
title: windows10NetworkProxyServer-Ressourcentyp
description: Netzwerk-Proxyserverrichtlinie.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dfe20e52ad63cf1d0d6a958f2ef5f4f89a53ad6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260697"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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



