---
title: omaSettingString-Ressourcentyp
description: Zeichenfolgendefinition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b32d5f6942dc5c0284e0ecaa11a27f4df0e99b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259913"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="10574-103">omaSettingString-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="10574-103">omaSettingString resource type</span></span>

> <span data-ttu-id="10574-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="10574-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10574-105">Zeichenfolgendefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="10574-105">OMA Settings String definition.</span></span>


<span data-ttu-id="10574-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="10574-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="10574-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10574-107">Properties</span></span>
|<span data-ttu-id="10574-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10574-108">Property</span></span>|<span data-ttu-id="10574-109">Typ</span><span class="sxs-lookup"><span data-stu-id="10574-109">Type</span></span>|<span data-ttu-id="10574-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10574-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10574-111">displayName</span><span class="sxs-lookup"><span data-stu-id="10574-111">displayName</span></span>|<span data-ttu-id="10574-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10574-112">String</span></span>|<span data-ttu-id="10574-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="10574-113">Display Name.</span></span> <span data-ttu-id="10574-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="10574-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="10574-115">description</span><span class="sxs-lookup"><span data-stu-id="10574-115">description</span></span>|<span data-ttu-id="10574-116">String</span><span class="sxs-lookup"><span data-stu-id="10574-116">String</span></span>|<span data-ttu-id="10574-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="10574-117">Description.</span></span> <span data-ttu-id="10574-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="10574-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="10574-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="10574-119">omaUri</span></span>|<span data-ttu-id="10574-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10574-120">String</span></span>|<span data-ttu-id="10574-121">OMA</span><span class="sxs-lookup"><span data-stu-id="10574-121">OMA.</span></span> <span data-ttu-id="10574-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="10574-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="10574-123">Wert</span><span class="sxs-lookup"><span data-stu-id="10574-123">value</span></span>|<span data-ttu-id="10574-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10574-124">String</span></span>|<span data-ttu-id="10574-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="10574-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10574-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="10574-126">Relationships</span></span>
<span data-ttu-id="10574-127">Keine</span><span class="sxs-lookup"><span data-stu-id="10574-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10574-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10574-128">JSON Representation</span></span>
<span data-ttu-id="10574-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="10574-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



