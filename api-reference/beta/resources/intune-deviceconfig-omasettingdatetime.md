---
title: omaSettingDateTime-Ressourcentyp
description: DateTime-Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 283b41018ad89b157c679c8b532c869d350b9182
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144464"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="efe90-103">omaSettingDateTime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="efe90-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="efe90-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="efe90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efe90-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="efe90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efe90-106">DateTime-Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="efe90-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="efe90-107">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="efe90-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="efe90-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="efe90-108">Properties</span></span>
|<span data-ttu-id="efe90-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="efe90-109">Property</span></span>|<span data-ttu-id="efe90-110">Typ</span><span class="sxs-lookup"><span data-stu-id="efe90-110">Type</span></span>|<span data-ttu-id="efe90-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efe90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efe90-112">displayName</span><span class="sxs-lookup"><span data-stu-id="efe90-112">displayName</span></span>|<span data-ttu-id="efe90-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="efe90-113">String</span></span>|<span data-ttu-id="efe90-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="efe90-114">Display Name.</span></span> <span data-ttu-id="efe90-115">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="efe90-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="efe90-116">description</span><span class="sxs-lookup"><span data-stu-id="efe90-116">description</span></span>|<span data-ttu-id="efe90-117">String</span><span class="sxs-lookup"><span data-stu-id="efe90-117">String</span></span>|<span data-ttu-id="efe90-118">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="efe90-118">Description.</span></span> <span data-ttu-id="efe90-119">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="efe90-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="efe90-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="efe90-120">omaUri</span></span>|<span data-ttu-id="efe90-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="efe90-121">String</span></span>|<span data-ttu-id="efe90-122">OMA</span><span class="sxs-lookup"><span data-stu-id="efe90-122">OMA.</span></span> <span data-ttu-id="efe90-123">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="efe90-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="efe90-124">Wert</span><span class="sxs-lookup"><span data-stu-id="efe90-124">value</span></span>|<span data-ttu-id="efe90-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efe90-125">DateTimeOffset</span></span>|<span data-ttu-id="efe90-126">Wert.</span><span class="sxs-lookup"><span data-stu-id="efe90-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efe90-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="efe90-127">Relationships</span></span>
<span data-ttu-id="efe90-128">Keine</span><span class="sxs-lookup"><span data-stu-id="efe90-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efe90-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="efe90-129">JSON Representation</span></span>
<span data-ttu-id="efe90-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="efe90-130">Here is a JSON representation of the resource.</span></span>
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




