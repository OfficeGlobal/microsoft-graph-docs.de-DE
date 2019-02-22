---
title: windowsInformationProtectionIPRangeCollection-Ressourcentyp
description: Windows Information Protection – IP-Bereichssammlung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cecc1b6bb2fae45da75123000b890654c7c52c2d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160690"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="3c007-103">windowsInformationProtectionIPRangeCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3c007-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="3c007-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c007-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c007-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3c007-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c007-106">Windows Information Protection – IP-Bereichssammlung</span><span class="sxs-lookup"><span data-stu-id="3c007-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="3c007-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c007-107">Properties</span></span>
|<span data-ttu-id="3c007-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c007-108">Property</span></span>|<span data-ttu-id="3c007-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3c007-109">Type</span></span>|<span data-ttu-id="3c007-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c007-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c007-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3c007-111">displayName</span></span>|<span data-ttu-id="3c007-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c007-112">String</span></span>|<span data-ttu-id="3c007-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="3c007-113">Display name</span></span>|
|<span data-ttu-id="3c007-114">ranges</span><span class="sxs-lookup"><span data-stu-id="3c007-114">ranges</span></span>|<span data-ttu-id="3c007-115">[ipRange](../resources/intune-shared-iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3c007-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="3c007-116">Sammlung der IP-Bereiche</span><span class="sxs-lookup"><span data-stu-id="3c007-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c007-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3c007-117">Relationships</span></span>
<span data-ttu-id="3c007-118">Keine</span><span class="sxs-lookup"><span data-stu-id="3c007-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c007-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c007-119">JSON Representation</span></span>
<span data-ttu-id="3c007-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c007-120">Here is a JSON representation of the resource.</span></span>
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




