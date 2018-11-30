---
title: windows10NetworkProxyServer-Ressourcentyp
description: Netzwerk-Proxyserverrichtlinie.
ms.openlocfilehash: 4e2e995c8d66249e5c742343f74e18e87337bfaa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063657"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="8e485-103">windows10NetworkProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e485-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="8e485-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8e485-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e485-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e485-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e485-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e485-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e485-107">Netzwerk-Proxyserverrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="8e485-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="8e485-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e485-108">Properties</span></span>
|<span data-ttu-id="8e485-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e485-109">Property</span></span>|<span data-ttu-id="8e485-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8e485-110">Type</span></span>|<span data-ttu-id="8e485-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e485-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e485-112">address</span><span class="sxs-lookup"><span data-stu-id="8e485-112">address</span></span>|<span data-ttu-id="8e485-113">String</span><span class="sxs-lookup"><span data-stu-id="8e485-113">String</span></span>|<span data-ttu-id="8e485-114">Adresse des Proxyservers.</span><span class="sxs-lookup"><span data-stu-id="8e485-114">Address to the proxy server.</span></span> <span data-ttu-id="8e485-115">Geben Sie eine Adresse im Format <server>\[":"<port>\] an.</span><span class="sxs-lookup"><span data-stu-id="8e485-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="8e485-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="8e485-116">exceptions</span></span>|<span data-ttu-id="8e485-117">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8e485-117">String collection</span></span>|<span data-ttu-id="8e485-118">Adressen, die den Proxyserver nicht verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="8e485-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="8e485-119">Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.</span><span class="sxs-lookup"><span data-stu-id="8e485-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="8e485-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="8e485-120">useForLocalAddresses</span></span>|<span data-ttu-id="8e485-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e485-121">Boolean</span></span>|<span data-ttu-id="8e485-122">Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8e485-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e485-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e485-123">Relationships</span></span>
<span data-ttu-id="8e485-124">Keine</span><span class="sxs-lookup"><span data-stu-id="8e485-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e485-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e485-125">JSON Representation</span></span>
<span data-ttu-id="8e485-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e485-126">Here is a JSON representation of the resource.</span></span>
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





