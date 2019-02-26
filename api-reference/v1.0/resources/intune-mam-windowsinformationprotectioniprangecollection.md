---
title: windowsInformationProtectionIPRangeCollection-Ressourcentyp
description: Windows Information Protection – IP-Bereichssammlung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6a2f52613eae9d8e06751672c95230dfc3b00c4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253897"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="b5ff0-103">windowsInformationProtectionIPRangeCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b5ff0-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="b5ff0-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b5ff0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5ff0-105">Windows Information Protection – IP-Bereichssammlung</span><span class="sxs-lookup"><span data-stu-id="b5ff0-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="b5ff0-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5ff0-106">Properties</span></span>
|<span data-ttu-id="b5ff0-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5ff0-107">Property</span></span>|<span data-ttu-id="b5ff0-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b5ff0-108">Type</span></span>|<span data-ttu-id="b5ff0-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5ff0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5ff0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b5ff0-110">displayName</span></span>|<span data-ttu-id="b5ff0-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5ff0-111">String</span></span>|<span data-ttu-id="b5ff0-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b5ff0-112">Display name</span></span>|
|<span data-ttu-id="b5ff0-113">ranges</span><span class="sxs-lookup"><span data-stu-id="b5ff0-113">ranges</span></span>|<span data-ttu-id="b5ff0-114">[ipRange](../resources/intune-mam-iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b5ff0-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="b5ff0-115">Sammlung von Internet Protokoll-Adressbereichen</span><span class="sxs-lookup"><span data-stu-id="b5ff0-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5ff0-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b5ff0-116">Relationships</span></span>
<span data-ttu-id="b5ff0-117">Keine</span><span class="sxs-lookup"><span data-stu-id="b5ff0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5ff0-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b5ff0-118">JSON Representation</span></span>
<span data-ttu-id="b5ff0-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b5ff0-119">Here is a JSON representation of the resource.</span></span>
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



