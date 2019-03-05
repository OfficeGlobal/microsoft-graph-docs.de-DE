---
title: omaSettingBoolean-Ressourcentyp
description: Boolesche Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d202997cdf0c1325e887337842513cc30dd2941
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256392"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="96c2d-103">omaSettingBoolean-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="96c2d-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="96c2d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="96c2d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96c2d-105">Boolesche Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="96c2d-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="96c2d-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="96c2d-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96c2d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96c2d-107">Properties</span></span>
|<span data-ttu-id="96c2d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96c2d-108">Property</span></span>|<span data-ttu-id="96c2d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="96c2d-109">Type</span></span>|<span data-ttu-id="96c2d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96c2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96c2d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="96c2d-111">displayName</span></span>|<span data-ttu-id="96c2d-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96c2d-112">String</span></span>|<span data-ttu-id="96c2d-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="96c2d-113">Display Name.</span></span> <span data-ttu-id="96c2d-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="96c2d-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="96c2d-115">description</span><span class="sxs-lookup"><span data-stu-id="96c2d-115">description</span></span>|<span data-ttu-id="96c2d-116">String</span><span class="sxs-lookup"><span data-stu-id="96c2d-116">String</span></span>|<span data-ttu-id="96c2d-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="96c2d-117">Description.</span></span> <span data-ttu-id="96c2d-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="96c2d-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="96c2d-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="96c2d-119">omaUri</span></span>|<span data-ttu-id="96c2d-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96c2d-120">String</span></span>|<span data-ttu-id="96c2d-121">OMA</span><span class="sxs-lookup"><span data-stu-id="96c2d-121">OMA.</span></span> <span data-ttu-id="96c2d-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="96c2d-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="96c2d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="96c2d-123">value</span></span>|<span data-ttu-id="96c2d-124">Boolescher</span><span class="sxs-lookup"><span data-stu-id="96c2d-124">Boolean</span></span>|<span data-ttu-id="96c2d-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="96c2d-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96c2d-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="96c2d-126">Relationships</span></span>
<span data-ttu-id="96c2d-127">Keine</span><span class="sxs-lookup"><span data-stu-id="96c2d-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96c2d-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96c2d-128">JSON Representation</span></span>
<span data-ttu-id="96c2d-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="96c2d-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



