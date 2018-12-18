---
title: windowsInformationProtectionIPRangeCollection-Ressourcentyp
description: Windows Information Protection – IP-Bereichssammlung
author: tfitzmac
ms.openlocfilehash: 6767a69ab1f3fe1b90c2a6b6fc7e76ea1abe2d99
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319054"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="9da44-103">windowsInformationProtectionIPRangeCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9da44-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="9da44-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9da44-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9da44-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9da44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9da44-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9da44-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9da44-107">Windows Information Protection – IP-Bereichssammlung</span><span class="sxs-lookup"><span data-stu-id="9da44-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="9da44-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9da44-108">Properties</span></span>
|<span data-ttu-id="9da44-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9da44-109">Property</span></span>|<span data-ttu-id="9da44-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9da44-110">Type</span></span>|<span data-ttu-id="9da44-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9da44-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9da44-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9da44-112">displayName</span></span>|<span data-ttu-id="9da44-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9da44-113">String</span></span>|<span data-ttu-id="9da44-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="9da44-114">Display name</span></span>|
|<span data-ttu-id="9da44-115">ranges</span><span class="sxs-lookup"><span data-stu-id="9da44-115">ranges</span></span>|<span data-ttu-id="9da44-116">[ipRange](../resources/intune-shared-iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9da44-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="9da44-117">Sammlung der IP-Bereiche</span><span class="sxs-lookup"><span data-stu-id="9da44-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="9da44-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9da44-118">Relationships</span></span>
<span data-ttu-id="9da44-119">Keine</span><span class="sxs-lookup"><span data-stu-id="9da44-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9da44-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9da44-120">JSON Representation</span></span>
<span data-ttu-id="9da44-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9da44-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```





