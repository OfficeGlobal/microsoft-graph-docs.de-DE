---
title: iPv6Range-Ressourcentyp
description: IPV6-Bereich
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c30d85a83bb604a5c0ccb6563d6315a183f6497
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971480"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="c8618-103">iPv6Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c8618-103">iPv6Range resource type</span></span>

> <span data-ttu-id="c8618-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c8618-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8618-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8618-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8618-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c8618-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8618-107">IPV6-Bereich</span><span class="sxs-lookup"><span data-stu-id="c8618-107">IP V6 range</span></span>

<span data-ttu-id="c8618-108">Erbt von [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c8618-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8618-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c8618-109">Properties</span></span>
|<span data-ttu-id="c8618-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8618-110">Property</span></span>|<span data-ttu-id="c8618-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c8618-111">Type</span></span>|<span data-ttu-id="c8618-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8618-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8618-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="c8618-113">lowerAddress</span></span>|<span data-ttu-id="c8618-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8618-114">String</span></span>|<span data-ttu-id="c8618-115">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="c8618-115">Lower IP Address</span></span>|
|<span data-ttu-id="c8618-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="c8618-116">upperAddress</span></span>|<span data-ttu-id="c8618-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8618-117">String</span></span>|<span data-ttu-id="c8618-118">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="c8618-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8618-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c8618-119">Relationships</span></span>
<span data-ttu-id="c8618-120">Keine</span><span class="sxs-lookup"><span data-stu-id="c8618-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8618-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c8618-121">JSON Representation</span></span>
<span data-ttu-id="c8618-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c8618-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



