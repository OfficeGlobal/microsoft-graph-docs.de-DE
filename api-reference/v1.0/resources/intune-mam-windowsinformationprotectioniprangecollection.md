---
title: windowsInformationProtectionIPRangeCollection-Ressourcentyp
description: Windows Information Protection – IP-Bereichssammlung
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e9d23f8a6d771b116b35058c249866c70c7460d8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952657"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="19d37-103">windowsInformationProtectionIPRangeCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="19d37-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="19d37-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="19d37-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19d37-105">Windows Information Protection – IP-Bereichssammlung</span><span class="sxs-lookup"><span data-stu-id="19d37-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="19d37-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="19d37-106">Properties</span></span>
|<span data-ttu-id="19d37-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19d37-107">Property</span></span>|<span data-ttu-id="19d37-108">Typ</span><span class="sxs-lookup"><span data-stu-id="19d37-108">Type</span></span>|<span data-ttu-id="19d37-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19d37-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19d37-110">displayName</span><span class="sxs-lookup"><span data-stu-id="19d37-110">displayName</span></span>|<span data-ttu-id="19d37-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19d37-111">String</span></span>|<span data-ttu-id="19d37-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="19d37-112">Display name</span></span>|
|<span data-ttu-id="19d37-113">ranges</span><span class="sxs-lookup"><span data-stu-id="19d37-113">ranges</span></span>|<span data-ttu-id="19d37-114">[ipRange](../resources/intune-mam-iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="19d37-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="19d37-115">Sammlung der IP-Bereiche</span><span class="sxs-lookup"><span data-stu-id="19d37-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="19d37-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="19d37-116">Relationships</span></span>
<span data-ttu-id="19d37-117">Keine</span><span class="sxs-lookup"><span data-stu-id="19d37-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19d37-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="19d37-118">JSON Representation</span></span>
<span data-ttu-id="19d37-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="19d37-119">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



