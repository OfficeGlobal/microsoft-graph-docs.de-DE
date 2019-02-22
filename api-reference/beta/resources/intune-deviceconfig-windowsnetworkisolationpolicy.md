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
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="85945-103">windowsNetworkIsolationPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="85945-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="85945-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85945-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85945-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="85945-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85945-106">Windows-Netzwerk Isolations Richtlinie</span><span class="sxs-lookup"><span data-stu-id="85945-106">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="85945-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85945-107">Properties</span></span>
|<span data-ttu-id="85945-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85945-108">Property</span></span>|<span data-ttu-id="85945-109">Typ</span><span class="sxs-lookup"><span data-stu-id="85945-109">Type</span></span>|<span data-ttu-id="85945-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85945-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85945-111">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="85945-111">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="85945-112">String collection</span><span class="sxs-lookup"><span data-stu-id="85945-112">String collection</span></span>|<span data-ttu-id="85945-113">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="85945-113">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="85945-114">Daten aus einer dieser Domänen, die an ein Gerät gesendet werden, werden als Unternehmensdaten betrachtet und geschützt.</span><span class="sxs-lookup"><span data-stu-id="85945-114">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="85945-115">Diese Standorte werden als sicheres Ziel für die Freigabe von Enterprise-Daten betrachtet.</span><span class="sxs-lookup"><span data-stu-id="85945-115">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="85945-116">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="85945-116">enterpriseCloudResources</span></span>|<span data-ttu-id="85945-117">[proxiedDomain](../resources/intune-shared-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85945-117">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="85945-118">Enthält eine Liste der in der Cloud gehosteten Enterprise-Ressourcendomänen, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="85945-118">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="85945-119">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="85945-119">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="85945-120">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="85945-120">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="85945-121">Ein zu diesem Zweck verwendeter Proxy Server muss auch mithilfe der EnterpriseInternalProxyServers-Richtlinie konfiguriert werden.</span><span class="sxs-lookup"><span data-stu-id="85945-121">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="85945-122">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="85945-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="85945-123">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="85945-123">enterpriseIPRanges</span></span>|<span data-ttu-id="85945-124">[ipRange](../resources/intune-shared-iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="85945-124">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="85945-125">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="85945-125">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="85945-126">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="85945-126">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="85945-127">Diese Standorte werden als sicheres Ziel für die Freigabe von Enterprise-Daten betrachtet.</span><span class="sxs-lookup"><span data-stu-id="85945-127">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="85945-128">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="85945-128">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="85945-129">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="85945-129">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="85945-130">String collection</span><span class="sxs-lookup"><span data-stu-id="85945-130">String collection</span></span>|<span data-ttu-id="85945-131">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="85945-131">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="85945-132">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="85945-132">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="85945-133">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="85945-133">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="85945-134">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="85945-134">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="85945-135">Die Proxys werden nur bei der Konfiguration der EnterpriseCloudResources-Richtlinie genutzt, um den Datenverkehr zu den zugeordneten Cloud-Ressourcen über diese Proxys zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="85945-135">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="85945-136">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="85945-136">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="85945-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="85945-137">Boolean</span></span>|<span data-ttu-id="85945-138">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="85945-138">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="85945-139">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="85945-139">Default is false.</span></span>|
|<span data-ttu-id="85945-140">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="85945-140">enterpriseProxyServers</span></span>|<span data-ttu-id="85945-141">String collection</span><span class="sxs-lookup"><span data-stu-id="85945-141">String collection</span></span>|<span data-ttu-id="85945-142">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="85945-142">This is a list of proxy servers.</span></span> <span data-ttu-id="85945-143">Jeder Server, der nicht in dieser Liste aufgeführt ist, wird als nicht-Enterprise angesehen.</span><span class="sxs-lookup"><span data-stu-id="85945-143">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="85945-144">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="85945-144">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="85945-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="85945-145">Boolean</span></span>|<span data-ttu-id="85945-146">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="85945-146">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="85945-147">Der Standardwert ist „FALSE“.</span><span class="sxs-lookup"><span data-stu-id="85945-147">Default is false</span></span>|
|<span data-ttu-id="85945-148">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="85945-148">neutralDomainResources</span></span>|<span data-ttu-id="85945-149">String collection</span><span class="sxs-lookup"><span data-stu-id="85945-149">String collection</span></span>|<span data-ttu-id="85945-150">Liste der Domänennamen, die für Arbeits-oder persönliche Ressourcen verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="85945-150">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85945-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="85945-151">Relationships</span></span>
<span data-ttu-id="85945-152">Keine</span><span class="sxs-lookup"><span data-stu-id="85945-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85945-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85945-153">JSON Representation</span></span>
<span data-ttu-id="85945-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="85945-154">Here is a JSON representation of the resource.</span></span>
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




