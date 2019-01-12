---
title: iPv4Range-Ressourcentyp
description: IP-V4-Bereich
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c260796259ce6084add7eadb48192ea50c209c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931930"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="42c52-103">iPv4Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="42c52-103">iPv4Range resource type</span></span>

> <span data-ttu-id="42c52-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="42c52-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42c52-105">IP-V4-Bereich</span><span class="sxs-lookup"><span data-stu-id="42c52-105">IP V4 range</span></span>

<span data-ttu-id="42c52-106">Erbt von [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="42c52-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42c52-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42c52-107">Properties</span></span>
|<span data-ttu-id="42c52-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42c52-108">Property</span></span>|<span data-ttu-id="42c52-109">Typ</span><span class="sxs-lookup"><span data-stu-id="42c52-109">Type</span></span>|<span data-ttu-id="42c52-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42c52-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42c52-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="42c52-111">lowerAddress</span></span>|<span data-ttu-id="42c52-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42c52-112">String</span></span>|<span data-ttu-id="42c52-113">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="42c52-113">Lower IP Address</span></span>|
|<span data-ttu-id="42c52-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="42c52-114">upperAddress</span></span>|<span data-ttu-id="42c52-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42c52-115">String</span></span>|<span data-ttu-id="42c52-116">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="42c52-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="42c52-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="42c52-117">Relationships</span></span>
<span data-ttu-id="42c52-118">Keine</span><span class="sxs-lookup"><span data-stu-id="42c52-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42c52-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="42c52-119">JSON Representation</span></span>
<span data-ttu-id="42c52-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42c52-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



