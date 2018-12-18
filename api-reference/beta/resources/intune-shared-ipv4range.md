---
title: iPv4Range-Ressourcentyp
description: IP-V4-Bereich
author: tfitzmac
ms.openlocfilehash: eae240d185a6cf0dc2fc7d0d83194dc9f3f6f00d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314770"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="e82c4-103">iPv4Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e82c4-103">iPv4Range resource type</span></span>

> <span data-ttu-id="e82c4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e82c4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e82c4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e82c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e82c4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e82c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e82c4-107">IP-V4-Bereich</span><span class="sxs-lookup"><span data-stu-id="e82c4-107">IP V4 range</span></span>

<span data-ttu-id="e82c4-108">Erbt von [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e82c4-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e82c4-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e82c4-109">Properties</span></span>
|<span data-ttu-id="e82c4-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e82c4-110">Property</span></span>|<span data-ttu-id="e82c4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e82c4-111">Type</span></span>|<span data-ttu-id="e82c4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e82c4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e82c4-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="e82c4-113">lowerAddress</span></span>|<span data-ttu-id="e82c4-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e82c4-114">String</span></span>|<span data-ttu-id="e82c4-115">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="e82c4-115">Lower IP Address</span></span>|
|<span data-ttu-id="e82c4-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="e82c4-116">upperAddress</span></span>|<span data-ttu-id="e82c4-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e82c4-117">String</span></span>|<span data-ttu-id="e82c4-118">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="e82c4-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="e82c4-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e82c4-119">Relationships</span></span>
<span data-ttu-id="e82c4-120">Keine</span><span class="sxs-lookup"><span data-stu-id="e82c4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e82c4-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e82c4-121">JSON Representation</span></span>
<span data-ttu-id="e82c4-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e82c4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



