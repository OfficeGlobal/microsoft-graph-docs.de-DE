---
title: vpnRoute-Ressourcentyp
description: Definition der VPN-Route.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54706d47267eef8fff6c465f24e4e9caa183ccc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154299"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="667df-103">vpnRoute-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="667df-103">vpnRoute resource type</span></span>

> <span data-ttu-id="667df-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="667df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="667df-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="667df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="667df-106">Definition der VPN-Route.</span><span class="sxs-lookup"><span data-stu-id="667df-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="667df-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="667df-107">Properties</span></span>
|<span data-ttu-id="667df-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="667df-108">Property</span></span>|<span data-ttu-id="667df-109">Typ</span><span class="sxs-lookup"><span data-stu-id="667df-109">Type</span></span>|<span data-ttu-id="667df-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="667df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="667df-111">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="667df-111">destinationPrefix</span></span>|<span data-ttu-id="667df-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="667df-112">String</span></span>|<span data-ttu-id="667df-113">Ziel Präfix (IPv4/V6-Adresse).</span><span class="sxs-lookup"><span data-stu-id="667df-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="667df-114">prefixSize</span><span class="sxs-lookup"><span data-stu-id="667df-114">prefixSize</span></span>|<span data-ttu-id="667df-115">Int32</span><span class="sxs-lookup"><span data-stu-id="667df-115">Int32</span></span>|<span data-ttu-id="667df-116">Präfix Größe.</span><span class="sxs-lookup"><span data-stu-id="667df-116">Prefix size.</span></span> <span data-ttu-id="667df-117">(1-32).</span><span class="sxs-lookup"><span data-stu-id="667df-117">(1-32).</span></span> <span data-ttu-id="667df-118">Gültige Werte 1 bis 32</span><span class="sxs-lookup"><span data-stu-id="667df-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="667df-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="667df-119">Relationships</span></span>
<span data-ttu-id="667df-120">Keine</span><span class="sxs-lookup"><span data-stu-id="667df-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="667df-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="667df-121">JSON Representation</span></span>
<span data-ttu-id="667df-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="667df-122">Here is a JSON representation of the resource.</span></span>
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




