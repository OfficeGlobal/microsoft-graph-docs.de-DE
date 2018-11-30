---
title: Ressourcentyp windowsNetworkIsolationPolicy
description: Windows-Isolation Netzwerkrichtlinien
ms.openlocfilehash: 89c7db0453c76f6ec5016a4701bf357e27c579bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061615"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="01dfe-103">Ressourcentyp windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="01dfe-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="01dfe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="01dfe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01dfe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01dfe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01dfe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="01dfe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01dfe-107">Windows-Isolation Netzwerkrichtlinien</span><span class="sxs-lookup"><span data-stu-id="01dfe-107">Windows Network Isolation Policy</span></span>
## <a name="properties"></a><span data-ttu-id="01dfe-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="01dfe-108">Properties</span></span>
|<span data-ttu-id="01dfe-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01dfe-109">Property</span></span>|<span data-ttu-id="01dfe-110">Typ</span><span class="sxs-lookup"><span data-stu-id="01dfe-110">Type</span></span>|<span data-ttu-id="01dfe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01dfe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01dfe-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="01dfe-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="01dfe-113">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="01dfe-113">String collection</span></span>|<span data-ttu-id="01dfe-114">Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren.</span><span class="sxs-lookup"><span data-stu-id="01dfe-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="01dfe-115">Daten von einem diese Domänen, die zu einem Gerät gesendet wird werden als Enterprise-Daten und geschützt.</span><span class="sxs-lookup"><span data-stu-id="01dfe-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="01dfe-116">Diese Speicherorte gilt ein sicherer Ziel für die Enterprise-Daten auf freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="01dfe-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="01dfe-117">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="01dfe-117">enterpriseCloudResources</span></span>|<span data-ttu-id="01dfe-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="01dfe-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="01dfe-119">Enthält eine Liste der Enterprise-Ressourcendomänen gehostet in der Cloud, die geschützt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="01dfe-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="01dfe-120">Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten.</span><span class="sxs-lookup"><span data-stu-id="01dfe-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="01dfe-121">Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80).</span><span class="sxs-lookup"><span data-stu-id="01dfe-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="01dfe-122">Mit der Richtlinie EnterpriseInternalProxyServers muss auch für diesen Zweck verwendet ein Proxy-Server konfiguriert werden.</span><span class="sxs-lookup"><span data-stu-id="01dfe-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="01dfe-123">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="01dfe-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="01dfe-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="01dfe-124">enterpriseIPRanges</span></span>|<span data-ttu-id="01dfe-125">[ipRange](../resources/intune-shared-iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="01dfe-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="01dfe-126">Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren.</span><span class="sxs-lookup"><span data-stu-id="01dfe-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="01dfe-127">Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt.</span><span class="sxs-lookup"><span data-stu-id="01dfe-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="01dfe-128">Diese Speicherorte gilt ein sicherer Ziel für die Enterprise-Daten auf freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="01dfe-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="01dfe-129">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="01dfe-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="01dfe-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="01dfe-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="01dfe-131">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="01dfe-131">String collection</span></span>|<span data-ttu-id="01dfe-132">Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver.</span><span class="sxs-lookup"><span data-stu-id="01dfe-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="01dfe-133">Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“.</span><span class="sxs-lookup"><span data-stu-id="01dfe-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="01dfe-134">Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="01dfe-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="01dfe-135">Sie gelten als Adressen im Unternehmensnetzwerk.</span><span class="sxs-lookup"><span data-stu-id="01dfe-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="01dfe-136">Die Proxys sind nur in Konfigurieren der Richtlinie EnterpriseCloudResources, um Datenverkehr an die übereinstimmenden Cloudressourcen über diese Proxys erzwingen genutzt.</span><span class="sxs-lookup"><span data-stu-id="01dfe-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="01dfe-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="01dfe-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="01dfe-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="01dfe-138">Boolean</span></span>|<span data-ttu-id="01dfe-139">Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden.</span><span class="sxs-lookup"><span data-stu-id="01dfe-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="01dfe-140">Standard ist false.</span><span class="sxs-lookup"><span data-stu-id="01dfe-140">Default is false.</span></span>|
|<span data-ttu-id="01dfe-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="01dfe-141">enterpriseProxyServers</span></span>|<span data-ttu-id="01dfe-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="01dfe-142">String collection</span></span>|<span data-ttu-id="01dfe-143">Dies ist eine Liste von Proxyservern.</span><span class="sxs-lookup"><span data-stu-id="01dfe-143">This is a list of proxy servers.</span></span> <span data-ttu-id="01dfe-144">Jeder Server wird in dieser Liste nicht-Enterprise nicht berücksichtigt.</span><span class="sxs-lookup"><span data-stu-id="01dfe-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="01dfe-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="01dfe-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="01dfe-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="01dfe-146">Boolean</span></span>|<span data-ttu-id="01dfe-147">Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden.</span><span class="sxs-lookup"><span data-stu-id="01dfe-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="01dfe-148">Der Standardwert ist „FALSE“.</span><span class="sxs-lookup"><span data-stu-id="01dfe-148">Default is false</span></span>|
|<span data-ttu-id="01dfe-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="01dfe-149">neutralDomainResources</span></span>|<span data-ttu-id="01dfe-150">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="01dfe-150">String collection</span></span>|<span data-ttu-id="01dfe-151">Liste der Domänennamen, die für die Arbeit "oder" Persönliche Ressource verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="01dfe-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01dfe-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="01dfe-152">Relationships</span></span>
<span data-ttu-id="01dfe-153">Keine</span><span class="sxs-lookup"><span data-stu-id="01dfe-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="01dfe-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="01dfe-154">JSON Representation</span></span>
<span data-ttu-id="01dfe-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="01dfe-155">Here is a JSON representation of the resource.</span></span>
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





