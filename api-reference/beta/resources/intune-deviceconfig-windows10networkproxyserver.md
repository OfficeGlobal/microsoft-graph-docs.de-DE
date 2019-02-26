---
title: windows10NetworkProxyServer-Ressourcentyp
description: Netzwerk-Proxyserverrichtlinie.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f29c69789f6b2a4d41bbb5179ff71f721c64c88f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162104"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="401ca-103">windows10NetworkProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="401ca-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="401ca-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="401ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="401ca-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="401ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="401ca-106">Netzwerk-Proxyserverrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="401ca-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="401ca-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="401ca-107">Properties</span></span>
|<span data-ttu-id="401ca-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="401ca-108">Property</span></span>|<span data-ttu-id="401ca-109">Typ</span><span class="sxs-lookup"><span data-stu-id="401ca-109">Type</span></span>|<span data-ttu-id="401ca-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="401ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="401ca-111">address</span><span class="sxs-lookup"><span data-stu-id="401ca-111">address</span></span>|<span data-ttu-id="401ca-112">String</span><span class="sxs-lookup"><span data-stu-id="401ca-112">String</span></span>|<span data-ttu-id="401ca-113">Adresse des Proxyservers.</span><span class="sxs-lookup"><span data-stu-id="401ca-113">Address to the proxy server.</span></span> <span data-ttu-id="401ca-114">Geben Sie eine Adresse im Format <server>\[":"<port>\] an.</span><span class="sxs-lookup"><span data-stu-id="401ca-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="401ca-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="401ca-115">exceptions</span></span>|<span data-ttu-id="401ca-116">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="401ca-116">String collection</span></span>|<span data-ttu-id="401ca-117">Adressen, die den Proxyserver nicht verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="401ca-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="401ca-118">Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.</span><span class="sxs-lookup"><span data-stu-id="401ca-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="401ca-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="401ca-119">useForLocalAddresses</span></span>|<span data-ttu-id="401ca-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="401ca-120">Boolean</span></span>|<span data-ttu-id="401ca-121">Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="401ca-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="401ca-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="401ca-122">Relationships</span></span>
<span data-ttu-id="401ca-123">Keine</span><span class="sxs-lookup"><span data-stu-id="401ca-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="401ca-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="401ca-124">JSON Representation</span></span>
<span data-ttu-id="401ca-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="401ca-125">Here is a JSON representation of the resource.</span></span>
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




