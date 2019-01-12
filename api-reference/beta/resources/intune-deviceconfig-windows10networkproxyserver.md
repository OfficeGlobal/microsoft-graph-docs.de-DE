---
title: windows10NetworkProxyServer-Ressourcentyp
description: Netzwerk-Proxyserverrichtlinie.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c193c5b5d1ba61626bb348f52caf39ded58a77c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951915"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="a8f0a-103">windows10NetworkProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a8f0a-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="a8f0a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8f0a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8f0a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8f0a-107">Netzwerk-Proxyserverrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="a8f0a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8f0a-108">Properties</span></span>
|<span data-ttu-id="a8f0a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8f0a-109">Property</span></span>|<span data-ttu-id="a8f0a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a8f0a-110">Type</span></span>|<span data-ttu-id="a8f0a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8f0a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8f0a-112">address</span><span class="sxs-lookup"><span data-stu-id="a8f0a-112">address</span></span>|<span data-ttu-id="a8f0a-113">String</span><span class="sxs-lookup"><span data-stu-id="a8f0a-113">String</span></span>|<span data-ttu-id="a8f0a-114">Adresse des Proxyservers.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-114">Address to the proxy server.</span></span> <span data-ttu-id="a8f0a-115">Geben Sie eine Adresse im Format <server>\[":"<port>\] an.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="a8f0a-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="a8f0a-116">exceptions</span></span>|<span data-ttu-id="a8f0a-117">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a8f0a-117">String collection</span></span>|<span data-ttu-id="a8f0a-118">Adressen, die den Proxyserver nicht verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="a8f0a-119">Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="a8f0a-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="a8f0a-120">useForLocalAddresses</span></span>|<span data-ttu-id="a8f0a-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8f0a-121">Boolean</span></span>|<span data-ttu-id="a8f0a-122">Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8f0a-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a8f0a-123">Relationships</span></span>
<span data-ttu-id="a8f0a-124">Keine</span><span class="sxs-lookup"><span data-stu-id="a8f0a-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8f0a-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8f0a-125">JSON Representation</span></span>
<span data-ttu-id="a8f0a-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8f0a-126">Here is a JSON representation of the resource.</span></span>
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





