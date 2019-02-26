---
title: omaSettingDateTime-Ressourcentyp
description: DateTime-Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20bc82e88480dca1df727e299e62c4274002176f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260914"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="4738b-103">omaSettingDateTime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4738b-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="4738b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4738b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4738b-105">DateTime-Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="4738b-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="4738b-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="4738b-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4738b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4738b-107">Properties</span></span>
|<span data-ttu-id="4738b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4738b-108">Property</span></span>|<span data-ttu-id="4738b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="4738b-109">Type</span></span>|<span data-ttu-id="4738b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4738b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4738b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4738b-111">displayName</span></span>|<span data-ttu-id="4738b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4738b-112">String</span></span>|<span data-ttu-id="4738b-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="4738b-113">Display Name.</span></span> <span data-ttu-id="4738b-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4738b-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4738b-115">description</span><span class="sxs-lookup"><span data-stu-id="4738b-115">description</span></span>|<span data-ttu-id="4738b-116">String</span><span class="sxs-lookup"><span data-stu-id="4738b-116">String</span></span>|<span data-ttu-id="4738b-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="4738b-117">Description.</span></span> <span data-ttu-id="4738b-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4738b-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4738b-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4738b-119">omaUri</span></span>|<span data-ttu-id="4738b-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4738b-120">String</span></span>|<span data-ttu-id="4738b-121">OMA</span><span class="sxs-lookup"><span data-stu-id="4738b-121">OMA.</span></span> <span data-ttu-id="4738b-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4738b-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4738b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="4738b-123">value</span></span>|<span data-ttu-id="4738b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4738b-124">DateTimeOffset</span></span>|<span data-ttu-id="4738b-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="4738b-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4738b-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4738b-126">Relationships</span></span>
<span data-ttu-id="4738b-127">Keine</span><span class="sxs-lookup"><span data-stu-id="4738b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4738b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4738b-128">JSON Representation</span></span>
<span data-ttu-id="4738b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4738b-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



