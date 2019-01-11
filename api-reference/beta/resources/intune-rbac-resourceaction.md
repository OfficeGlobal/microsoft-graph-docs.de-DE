---
title: resourceAction-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d607ca2b250e9d2af55b74ef568a82c522bf761
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876384"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="e2740-103">resourceAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e2740-103">resourceAction resource type</span></span>

> <span data-ttu-id="e2740-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2740-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2740-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2740-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2740-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e2740-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2740-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e2740-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e2740-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2740-108">Properties</span></span>
|<span data-ttu-id="e2740-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2740-109">Property</span></span>|<span data-ttu-id="e2740-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e2740-110">Type</span></span>|<span data-ttu-id="e2740-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2740-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2740-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="e2740-112">allowedResourceActions</span></span>|<span data-ttu-id="e2740-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e2740-113">String collection</span></span>|<span data-ttu-id="e2740-114">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="e2740-114">Allowed Actions</span></span>|
|<span data-ttu-id="e2740-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="e2740-115">notAllowedResourceActions</span></span>|<span data-ttu-id="e2740-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e2740-116">String collection</span></span>|<span data-ttu-id="e2740-117">Nicht zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="e2740-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2740-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2740-118">Relationships</span></span>
<span data-ttu-id="e2740-119">Keine</span><span class="sxs-lookup"><span data-stu-id="e2740-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2740-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2740-120">JSON Representation</span></span>
<span data-ttu-id="e2740-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2740-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





