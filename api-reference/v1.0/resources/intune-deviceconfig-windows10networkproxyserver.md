---
title: windows10NetworkProxyServer-Ressourcentyp
description: Netzwerk-Proxyserverrichtlinie.
ms.openlocfilehash: 2cd9d4ddc84733e3985f718fd2d3ef86481d762e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016722"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="4aeb1-103">windows10NetworkProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4aeb1-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="4aeb1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4aeb1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4aeb1-105">Netzwerk-Proxyserverrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="4aeb1-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="4aeb1-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4aeb1-106">Properties</span></span>
|<span data-ttu-id="4aeb1-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4aeb1-107">Property</span></span>|<span data-ttu-id="4aeb1-108">Typ</span><span class="sxs-lookup"><span data-stu-id="4aeb1-108">Type</span></span>|<span data-ttu-id="4aeb1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4aeb1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4aeb1-110">address</span><span class="sxs-lookup"><span data-stu-id="4aeb1-110">address</span></span>|<span data-ttu-id="4aeb1-111">String</span><span class="sxs-lookup"><span data-stu-id="4aeb1-111">String</span></span>|<span data-ttu-id="4aeb1-112">Adresse des Proxyservers.</span><span class="sxs-lookup"><span data-stu-id="4aeb1-112">Address to the proxy server.</span></span> <span data-ttu-id="4aeb1-113">Geben Sie eine Adresse im Format <server>\[":"<port>\] an.</span><span class="sxs-lookup"><span data-stu-id="4aeb1-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="4aeb1-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="4aeb1-114">exceptions</span></span>|<span data-ttu-id="4aeb1-115">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4aeb1-115">String collection</span></span>|<span data-ttu-id="4aeb1-116">Adressen, die den Proxyserver nicht verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="4aeb1-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="4aeb1-117">Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.</span><span class="sxs-lookup"><span data-stu-id="4aeb1-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="4aeb1-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="4aeb1-118">useForLocalAddresses</span></span>|<span data-ttu-id="4aeb1-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aeb1-119">Boolean</span></span>|<span data-ttu-id="4aeb1-120">Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4aeb1-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4aeb1-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4aeb1-121">Relationships</span></span>
<span data-ttu-id="4aeb1-122">Keine</span><span class="sxs-lookup"><span data-stu-id="4aeb1-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4aeb1-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4aeb1-123">JSON Representation</span></span>
<span data-ttu-id="4aeb1-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4aeb1-124">Here is a JSON representation of the resource.</span></span>
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



