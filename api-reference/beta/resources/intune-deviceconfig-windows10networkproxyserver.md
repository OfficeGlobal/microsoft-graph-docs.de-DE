---
title: windows10NetworkProxyServer-Ressourcentyp
description: Netzwerk-Proxyserverrichtlinie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 673cfe99e9cafe1b57fde5c70b7059286a6cc554
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418582"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="77465-103">windows10NetworkProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77465-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="77465-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="77465-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77465-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77465-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77465-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77465-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77465-107">Netzwerk-Proxyserverrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="77465-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="77465-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77465-108">Properties</span></span>
|<span data-ttu-id="77465-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77465-109">Property</span></span>|<span data-ttu-id="77465-110">Typ</span><span class="sxs-lookup"><span data-stu-id="77465-110">Type</span></span>|<span data-ttu-id="77465-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77465-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77465-112">address</span><span class="sxs-lookup"><span data-stu-id="77465-112">address</span></span>|<span data-ttu-id="77465-113">String</span><span class="sxs-lookup"><span data-stu-id="77465-113">String</span></span>|<span data-ttu-id="77465-114">Adresse des Proxyservers.</span><span class="sxs-lookup"><span data-stu-id="77465-114">Address to the proxy server.</span></span> <span data-ttu-id="77465-115">Geben Sie eine Adresse im Format <server>\[":"<port>\] an.</span><span class="sxs-lookup"><span data-stu-id="77465-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="77465-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="77465-116">exceptions</span></span>|<span data-ttu-id="77465-117">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="77465-117">String collection</span></span>|<span data-ttu-id="77465-118">Adressen, die den Proxyserver nicht verwenden sollten.</span><span class="sxs-lookup"><span data-stu-id="77465-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="77465-119">Das System verwendet den Proxyserver nicht für Adressen, die mit den Angaben in diesem Knoten beginnen.</span><span class="sxs-lookup"><span data-stu-id="77465-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="77465-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="77465-120">useForLocalAddresses</span></span>|<span data-ttu-id="77465-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="77465-121">Boolean</span></span>|<span data-ttu-id="77465-122">Gibt an, ob der Proxyserver für lokale (Intranet-)Adressen verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="77465-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77465-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77465-123">Relationships</span></span>
<span data-ttu-id="77465-124">Keine</span><span class="sxs-lookup"><span data-stu-id="77465-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77465-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77465-125">JSON Representation</span></span>
<span data-ttu-id="77465-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77465-126">Here is a JSON representation of the resource.</span></span>
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




