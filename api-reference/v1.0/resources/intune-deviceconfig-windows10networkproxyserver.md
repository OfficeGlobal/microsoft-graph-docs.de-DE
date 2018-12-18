---
title: windows10NetworkProxyServer-Ressourcentyp
description: Netzwerk-Proxyserverrichtlinie.
author: tfitzmac
ms.openlocfilehash: c2eaeaa4d89f981e5fa992e7a79a7863f0848a9f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344037"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="8104c-103">windows10NetworkProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8104c-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="8104c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8104c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8104c-105">Netzwerk-Proxyserverrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="8104c-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="8104c-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8104c-106">Properties</span></span>
|<span data-ttu-id="8104c-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8104c-107">Property</span></span>|<span data-ttu-id="8104c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8104c-108">Type</span></span>|<span data-ttu-id="8104c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8104c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8104c-110">address</span><span class="sxs-lookup"><span data-stu-id="8104c-110">address</span></span>|<span data-ttu-id="8104c-111">String</span><span class="sxs-lookup"><span data-stu-id="8104c-111">String</span></span>|<span data-ttu-id="8104c-112">Adresse des Proxyservers.</span><span class="sxs-lookup"><span data-stu-id="8104c-112">Address to the proxy server.</span></span> <span data-ttu-id="8104c-113">Geben Sie eine Adresse im Format <server>\[":"<port>\] an.</span><span class="sxs-lookup"><span data-stu-id="8104c-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="8104c-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="8104c-114">exceptions</span></span>|<span data-ttu-id="8104c-115">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8104c-115">String collection</span></span>|<span data-ttu-id="8104c-116">Adressen, die den Proxyserver nicht verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="8104c-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="8104c-117">Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.</span><span class="sxs-lookup"><span data-stu-id="8104c-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="8104c-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="8104c-118">useForLocalAddresses</span></span>|<span data-ttu-id="8104c-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8104c-119">Boolean</span></span>|<span data-ttu-id="8104c-120">Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8104c-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8104c-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8104c-121">Relationships</span></span>
<span data-ttu-id="8104c-122">Keine</span><span class="sxs-lookup"><span data-stu-id="8104c-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8104c-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8104c-123">JSON Representation</span></span>
<span data-ttu-id="8104c-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8104c-124">Here is a JSON representation of the resource.</span></span>
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



