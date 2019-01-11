---
title: iPv6Range-Ressourcentyp
description: IPV6-Bereich
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 759f661464d2dd5cd6c12f6fbfe6b1bfcf549a70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829659"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="1d980-103">iPv6Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1d980-103">iPv6Range resource type</span></span>

> <span data-ttu-id="1d980-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d980-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d980-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d980-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d980-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d980-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d980-107">IPV6-Bereich</span><span class="sxs-lookup"><span data-stu-id="1d980-107">IP V6 range</span></span>

<span data-ttu-id="1d980-108">Erbt von [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="1d980-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1d980-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d980-109">Properties</span></span>
|<span data-ttu-id="1d980-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d980-110">Property</span></span>|<span data-ttu-id="1d980-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1d980-111">Type</span></span>|<span data-ttu-id="1d980-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d980-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d980-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="1d980-113">lowerAddress</span></span>|<span data-ttu-id="1d980-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1d980-114">String</span></span>|<span data-ttu-id="1d980-115">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="1d980-115">Lower IP Address</span></span>|
|<span data-ttu-id="1d980-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="1d980-116">upperAddress</span></span>|<span data-ttu-id="1d980-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1d980-117">String</span></span>|<span data-ttu-id="1d980-118">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="1d980-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d980-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1d980-119">Relationships</span></span>
<span data-ttu-id="1d980-120">Keine</span><span class="sxs-lookup"><span data-stu-id="1d980-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d980-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d980-121">JSON Representation</span></span>
<span data-ttu-id="1d980-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1d980-122">Here is a JSON representation of the resource.</span></span>
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



