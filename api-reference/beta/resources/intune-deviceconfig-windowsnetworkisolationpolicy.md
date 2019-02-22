---
title: windowsNetworkIsolationPolicy-Ressourcentyp
description: Windows-Netzwerk Isolations Richtlinie
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e98d14d68ff5b936a9baf0a0065d0080f275a2ac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158240"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>windowsNetworkIsolationPolicy-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Windows-Netzwerk Isolations Richtlinie

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|enterpriseNetworkDomainNames|String collection|Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren. Daten aus einer dieser Domänen, die an ein Gerät gesendet werden, werden als Unternehmensdaten betrachtet und geschützt. Diese Standorte werden als sicheres Ziel für die Freigabe von Enterprise-Daten betrachtet.|
|enterpriseCloudResources|[proxiedDomain](../resources/intune-shared-proxieddomain.md)-Sammlung|Enthält eine Liste der in der Cloud gehosteten Enterprise-Ressourcendomänen, die geschützt werden müssen. Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten. Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80). Ein zu diesem Zweck verwendeter Proxy Server muss auch mithilfe der EnterpriseInternalProxyServers-Richtlinie konfiguriert werden. Diese Collection darf maximal 500 Elemente enthalten.|
|enterpriseIPRanges|[ipRange](../resources/intune-shared-iprange.md)-Sammlung|Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren. Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt. Diese Standorte werden als sicheres Ziel für die Freigabe von Enterprise-Daten betrachtet. Diese Collection darf maximal 500 Elemente enthalten.|
|enterpriseInternalProxyServers|String collection|Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver. Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“. Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert. Sie gelten als Adressen im Unternehmensnetzwerk. Die Proxys werden nur bei der Konfiguration der EnterpriseCloudResources-Richtlinie genutzt, um den Datenverkehr zu den zugeordneten Cloud-Ressourcen über diese Proxys zu erzwingen.|
|enterpriseIPRangesAreAuthoritative|Boolescher Wert|Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden. Der Standardwert ist false.|
|enterpriseProxyServers|String collection|Dies ist eine Liste von Proxyservern. Jeder Server, der nicht in dieser Liste aufgeführt ist, wird als nicht-Enterprise angesehen.|
|enterpriseProxyServersAreAuthoritative|Boolescher Wert|Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden. Der Standardwert ist „FALSE“.|
|neutralDomainResources|String collection|Liste der Domänennamen, die für Arbeits-oder persönliche Ressourcen verwendet werden können.|

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




