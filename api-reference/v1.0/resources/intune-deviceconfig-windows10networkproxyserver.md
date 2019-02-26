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
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="450f3-103">windows10NetworkProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="450f3-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="450f3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="450f3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="450f3-105">Netzwerk-Proxyserverrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="450f3-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="450f3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="450f3-106">Properties</span></span>
|<span data-ttu-id="450f3-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="450f3-107">Property</span></span>|<span data-ttu-id="450f3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="450f3-108">Type</span></span>|<span data-ttu-id="450f3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="450f3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="450f3-110">address</span><span class="sxs-lookup"><span data-stu-id="450f3-110">address</span></span>|<span data-ttu-id="450f3-111">String</span><span class="sxs-lookup"><span data-stu-id="450f3-111">String</span></span>|<span data-ttu-id="450f3-112">Adresse des Proxyservers.</span><span class="sxs-lookup"><span data-stu-id="450f3-112">Address to the proxy server.</span></span> <span data-ttu-id="450f3-113">Geben Sie eine Adresse im Format <server>\[":"<port>\] an.</span><span class="sxs-lookup"><span data-stu-id="450f3-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="450f3-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="450f3-114">exceptions</span></span>|<span data-ttu-id="450f3-115">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="450f3-115">String collection</span></span>|<span data-ttu-id="450f3-116">Adressen, die den Proxyserver nicht verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="450f3-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="450f3-117">Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.</span><span class="sxs-lookup"><span data-stu-id="450f3-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="450f3-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="450f3-118">useForLocalAddresses</span></span>|<span data-ttu-id="450f3-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="450f3-119">Boolean</span></span>|<span data-ttu-id="450f3-120">Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="450f3-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="450f3-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="450f3-121">Relationships</span></span>
<span data-ttu-id="450f3-122">Keine</span><span class="sxs-lookup"><span data-stu-id="450f3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="450f3-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="450f3-123">JSON Representation</span></span>
<span data-ttu-id="450f3-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="450f3-124">Here is a JSON representation of the resource.</span></span>
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



