---
title: resourceAction-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94a0ce30dc6e9607aa1531e7421af6b7a5500939
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870732"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="6294b-103">resourceAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6294b-103">resourceAction resource type</span></span>

> <span data-ttu-id="6294b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6294b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6294b-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6294b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6294b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6294b-106">Properties</span></span>
|<span data-ttu-id="6294b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6294b-107">Property</span></span>|<span data-ttu-id="6294b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="6294b-108">Type</span></span>|<span data-ttu-id="6294b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6294b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6294b-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="6294b-110">allowedResourceActions</span></span>|<span data-ttu-id="6294b-111">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="6294b-111">String collection</span></span>|<span data-ttu-id="6294b-112">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="6294b-112">Allowed Actions</span></span>|
|<span data-ttu-id="6294b-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="6294b-113">notAllowedResourceActions</span></span>|<span data-ttu-id="6294b-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="6294b-114">String collection</span></span>|<span data-ttu-id="6294b-115">Nicht zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="6294b-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="6294b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6294b-116">Relationships</span></span>
<span data-ttu-id="6294b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="6294b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6294b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6294b-118">JSON Representation</span></span>
<span data-ttu-id="6294b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6294b-119">Here is a JSON representation of the resource.</span></span>
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



