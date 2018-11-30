---
title: resourceAction-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 4cbfc149207f2f7589bd7e05075326641d4e8b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016103"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="47012-103">resourceAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="47012-103">resourceAction resource type</span></span>

> <span data-ttu-id="47012-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="47012-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47012-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="47012-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="47012-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="47012-106">Properties</span></span>
|<span data-ttu-id="47012-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47012-107">Property</span></span>|<span data-ttu-id="47012-108">Typ</span><span class="sxs-lookup"><span data-stu-id="47012-108">Type</span></span>|<span data-ttu-id="47012-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47012-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47012-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="47012-110">allowedResourceActions</span></span>|<span data-ttu-id="47012-111">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="47012-111">String collection</span></span>|<span data-ttu-id="47012-112">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="47012-112">Allowed Actions</span></span>|
|<span data-ttu-id="47012-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="47012-113">notAllowedResourceActions</span></span>|<span data-ttu-id="47012-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="47012-114">String collection</span></span>|<span data-ttu-id="47012-115">Nicht zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="47012-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="47012-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="47012-116">Relationships</span></span>
<span data-ttu-id="47012-117">Keine</span><span class="sxs-lookup"><span data-stu-id="47012-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47012-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="47012-118">JSON Representation</span></span>
<span data-ttu-id="47012-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="47012-119">Here is a JSON representation of the resource.</span></span>
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



