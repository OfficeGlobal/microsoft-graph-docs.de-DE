---
title: Ressourcentyp windowsNetworkIsolationPolicy
description: Windows-Isolation Netzwerkrichtlinien
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 82026ba4d82b85a0275f83bb729b495e17ff5d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834615"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>Ressourcentyp windowsNetworkIsolationPolicy

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows-Isolation Netzwerkrichtlinien
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|enterpriseNetworkDomainNames|Collection von Objekten des Typs „String“|Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren. Daten von einem diese Domänen, die zu einem Gerät gesendet wird werden als Enterprise-Daten und geschützt. Diese Speicherorte gilt ein sicherer Ziel für die Enterprise-Daten auf freigegeben werden.|
|enterpriseCloudResources|[proxiedDomain](../resources/intune-shared-proxieddomain.md)-Sammlung|Enthält eine Liste der Enterprise-Ressourcendomänen gehostet in der Cloud, die geschützt werden müssen. Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten. Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80). Mit der Richtlinie EnterpriseInternalProxyServers muss auch für diesen Zweck verwendet ein Proxy-Server konfiguriert werden. Diese Collection darf maximal 500 Elemente enthalten.|
|enterpriseIPRanges|[ipRange](../resources/intune-shared-iprange.md)-Sammlung|Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren. Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt. Diese Speicherorte gilt ein sicherer Ziel für die Enterprise-Daten auf freigegeben werden. Diese Collection darf maximal 500 Elemente enthalten.|
|enterpriseInternalProxyServers|Collection von Objekten des Typs „String“|Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver. Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“. Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert. Sie gelten als Adressen im Unternehmensnetzwerk. Die Proxys sind nur in Konfigurieren der Richtlinie EnterpriseCloudResources, um Datenverkehr an die übereinstimmenden Cloudressourcen über diese Proxys erzwingen genutzt.|
|enterpriseIPRangesAreAuthoritative|Boolescher Wert|Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden. Standard ist false.|
|enterpriseProxyServers|Collection von Objekten des Typs „String“|Dies ist eine Liste von Proxyservern. Jeder Server wird in dieser Liste nicht-Enterprise nicht berücksichtigt.|
|enterpriseProxyServersAreAuthoritative|Boolescher Wert|Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden. Der Standardwert ist „FALSE“.|
|neutralDomainResources|Collection von Objekten des Typs „String“|Liste der Domänennamen, die für die Arbeit "oder" Persönliche Ressource verwendet werden können.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```





