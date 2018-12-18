---
title: resourceAction-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: b64c1fb0ef49c2d7c47c88137bcca8ef89f6ad67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343918"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="c7679-103">resourceAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c7679-103">resourceAction resource type</span></span>

> <span data-ttu-id="c7679-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c7679-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7679-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c7679-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c7679-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7679-106">Properties</span></span>
|<span data-ttu-id="c7679-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7679-107">Property</span></span>|<span data-ttu-id="c7679-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c7679-108">Type</span></span>|<span data-ttu-id="c7679-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7679-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7679-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c7679-110">allowedResourceActions</span></span>|<span data-ttu-id="c7679-111">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c7679-111">String collection</span></span>|<span data-ttu-id="c7679-112">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="c7679-112">Allowed Actions</span></span>|
|<span data-ttu-id="c7679-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c7679-113">notAllowedResourceActions</span></span>|<span data-ttu-id="c7679-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c7679-114">String collection</span></span>|<span data-ttu-id="c7679-115">Nicht zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="c7679-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7679-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c7679-116">Relationships</span></span>
<span data-ttu-id="c7679-117">Keine</span><span class="sxs-lookup"><span data-stu-id="c7679-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7679-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7679-118">JSON Representation</span></span>
<span data-ttu-id="c7679-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7679-119">Here is a JSON representation of the resource.</span></span>
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



