---
title: omaSettingFloatingPoint-Ressourcentyp
description: Gleitkommadefinition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4720d635eeb119a2e1cacc741ab9c96f8ac55d4f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255031"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="990c9-103">omaSettingFloatingPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="990c9-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="990c9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="990c9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="990c9-105">Gleitkommadefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="990c9-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="990c9-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="990c9-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="990c9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="990c9-107">Properties</span></span>
|<span data-ttu-id="990c9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="990c9-108">Property</span></span>|<span data-ttu-id="990c9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="990c9-109">Type</span></span>|<span data-ttu-id="990c9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="990c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="990c9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="990c9-111">displayName</span></span>|<span data-ttu-id="990c9-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="990c9-112">String</span></span>|<span data-ttu-id="990c9-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="990c9-113">Display Name.</span></span> <span data-ttu-id="990c9-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="990c9-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="990c9-115">description</span><span class="sxs-lookup"><span data-stu-id="990c9-115">description</span></span>|<span data-ttu-id="990c9-116">String</span><span class="sxs-lookup"><span data-stu-id="990c9-116">String</span></span>|<span data-ttu-id="990c9-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="990c9-117">Description.</span></span> <span data-ttu-id="990c9-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="990c9-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="990c9-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="990c9-119">omaUri</span></span>|<span data-ttu-id="990c9-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="990c9-120">String</span></span>|<span data-ttu-id="990c9-121">OMA</span><span class="sxs-lookup"><span data-stu-id="990c9-121">OMA.</span></span> <span data-ttu-id="990c9-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="990c9-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="990c9-123">Wert</span><span class="sxs-lookup"><span data-stu-id="990c9-123">value</span></span>|<span data-ttu-id="990c9-124">Einzelner</span><span class="sxs-lookup"><span data-stu-id="990c9-124">Single</span></span>|<span data-ttu-id="990c9-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="990c9-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="990c9-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="990c9-126">Relationships</span></span>
<span data-ttu-id="990c9-127">Keine</span><span class="sxs-lookup"><span data-stu-id="990c9-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="990c9-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="990c9-128">JSON Representation</span></span>
<span data-ttu-id="990c9-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="990c9-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



