---
title: Ressourcentyp vpnRoute
description: VPN-Route Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43924b76a76060ac6576657d172757a503204a82
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927590"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="1f3ca-103">Ressourcentyp vpnRoute</span><span class="sxs-lookup"><span data-stu-id="1f3ca-103">vpnRoute resource type</span></span>

> <span data-ttu-id="1f3ca-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1f3ca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f3ca-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f3ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f3ca-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1f3ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f3ca-107">VPN-Route Definition.</span><span class="sxs-lookup"><span data-stu-id="1f3ca-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="1f3ca-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1f3ca-108">Properties</span></span>
|<span data-ttu-id="1f3ca-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f3ca-109">Property</span></span>|<span data-ttu-id="1f3ca-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1f3ca-110">Type</span></span>|<span data-ttu-id="1f3ca-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f3ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f3ca-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="1f3ca-112">destinationPrefix</span></span>|<span data-ttu-id="1f3ca-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f3ca-113">String</span></span>|<span data-ttu-id="1f3ca-114">Ziel-Präfix (/ v6 IPv4-Adresse).</span><span class="sxs-lookup"><span data-stu-id="1f3ca-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="1f3ca-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="1f3ca-115">prefixSize</span></span>|<span data-ttu-id="1f3ca-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1f3ca-116">Int32</span></span>|<span data-ttu-id="1f3ca-117">Präfix Größe.</span><span class="sxs-lookup"><span data-stu-id="1f3ca-117">Prefix size.</span></span> <span data-ttu-id="1f3ca-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="1f3ca-118">(1-32).</span></span> <span data-ttu-id="1f3ca-119">Gültige Werte 1 bis 32</span><span class="sxs-lookup"><span data-stu-id="1f3ca-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f3ca-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1f3ca-120">Relationships</span></span>
<span data-ttu-id="1f3ca-121">Keine</span><span class="sxs-lookup"><span data-stu-id="1f3ca-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f3ca-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1f3ca-122">JSON Representation</span></span>
<span data-ttu-id="1f3ca-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1f3ca-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```





