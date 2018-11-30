---
title: NetworkInterface-Ressourcentyp
description: Stellt eine Network Interface Card (NIC) Hosts zugeordnet.
ms.openlocfilehash: 7044b4f469e74424b0dc27ffa38c5feb081faa45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058845"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="f9387-103">NetworkInterface-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f9387-103">networkInterface resource type</span></span>

<span data-ttu-id="f9387-104">Stellt eine Network Interface Card (NIC) Hosts zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="f9387-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="f9387-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9387-105">Properties</span></span>

| <span data-ttu-id="f9387-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9387-106">Property</span></span>   | <span data-ttu-id="f9387-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f9387-107">Type</span></span> |<span data-ttu-id="f9387-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9387-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9387-109">description</span><span class="sxs-lookup"><span data-stu-id="f9387-109">description</span></span>|<span data-ttu-id="f9387-110">String</span><span class="sxs-lookup"><span data-stu-id="f9387-110">String</span></span>|<span data-ttu-id="f9387-111">Beschreibung der NIC (z. B. Ethernet-Adapter, WLAN-Adapter LAN-Verbindung \* <> # usw..).</span><span class="sxs-lookup"><span data-stu-id="f9387-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="f9387-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="f9387-112">ipV4Address</span></span>|<span data-ttu-id="f9387-113">String</span><span class="sxs-lookup"><span data-stu-id="f9387-113">String</span></span>|<span data-ttu-id="f9387-114">Letzte IPv4-Adresse zugeordneten dieser Netzwerkkarte</span><span class="sxs-lookup"><span data-stu-id="f9387-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="f9387-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="f9387-115">ipV6Address</span></span>|<span data-ttu-id="f9387-116">String</span><span class="sxs-lookup"><span data-stu-id="f9387-116">String</span></span>|<span data-ttu-id="f9387-117">Letzte Öffentliche (auch bekannt als global) IPv6-Adresse zugeordneten dieser Netzwerkkarte</span><span class="sxs-lookup"><span data-stu-id="f9387-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="f9387-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="f9387-118">localIpV6Address</span></span>|<span data-ttu-id="f9387-119">String</span><span class="sxs-lookup"><span data-stu-id="f9387-119">String</span></span>|<span data-ttu-id="f9387-120">Letzte (Link-Local oder Site-Local) IPv6 zugeordnete lokale Adresse diese Netzwerkkarte ein.</span><span class="sxs-lookup"><span data-stu-id="f9387-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="f9387-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="f9387-121">macAddress</span></span>|<span data-ttu-id="f9387-122">String</span><span class="sxs-lookup"><span data-stu-id="f9387-122">String</span></span>|<span data-ttu-id="f9387-123">MAC-Adresse der Netzwerkkarte auf diesem Host.</span><span class="sxs-lookup"><span data-stu-id="f9387-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9387-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9387-124">JSON representation</span></span>

<span data-ttu-id="f9387-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9387-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->