---
title: omaSettingBase64-Ressourcentyp
description: Base64-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f6eae88e7158d5fd8d09caadda9fee6778182a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166647"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="35df7-103">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="35df7-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="35df7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35df7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35df7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="35df7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35df7-106">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="35df7-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="35df7-107">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="35df7-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="35df7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35df7-108">Properties</span></span>
|<span data-ttu-id="35df7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35df7-109">Property</span></span>|<span data-ttu-id="35df7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="35df7-110">Type</span></span>|<span data-ttu-id="35df7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35df7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35df7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="35df7-112">displayName</span></span>|<span data-ttu-id="35df7-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35df7-113">String</span></span>|<span data-ttu-id="35df7-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="35df7-114">Display Name.</span></span> <span data-ttu-id="35df7-115">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="35df7-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="35df7-116">description</span><span class="sxs-lookup"><span data-stu-id="35df7-116">description</span></span>|<span data-ttu-id="35df7-117">String</span><span class="sxs-lookup"><span data-stu-id="35df7-117">String</span></span>|<span data-ttu-id="35df7-118">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="35df7-118">Description.</span></span> <span data-ttu-id="35df7-119">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="35df7-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="35df7-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="35df7-120">omaUri</span></span>|<span data-ttu-id="35df7-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35df7-121">String</span></span>|<span data-ttu-id="35df7-122">OMA</span><span class="sxs-lookup"><span data-stu-id="35df7-122">OMA.</span></span> <span data-ttu-id="35df7-123">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="35df7-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="35df7-124">fileName</span><span class="sxs-lookup"><span data-stu-id="35df7-124">fileName</span></span>|<span data-ttu-id="35df7-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35df7-125">String</span></span>|<span data-ttu-id="35df7-126">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="35df7-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="35df7-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="35df7-127">\*.crt</span></span> | <span data-ttu-id="35df7-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="35df7-128">\*.p7b</span></span> | <span data-ttu-id="35df7-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="35df7-129">\*.bin).</span></span>|
|<span data-ttu-id="35df7-130">Wert</span><span class="sxs-lookup"><span data-stu-id="35df7-130">value</span></span>|<span data-ttu-id="35df7-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="35df7-131">String</span></span>|<span data-ttu-id="35df7-132">Wert</span><span class="sxs-lookup"><span data-stu-id="35df7-132">Value.</span></span> <span data-ttu-id="35df7-133">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="35df7-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="35df7-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="35df7-134">Relationships</span></span>
<span data-ttu-id="35df7-135">Keine</span><span class="sxs-lookup"><span data-stu-id="35df7-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35df7-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35df7-136">JSON Representation</span></span>
<span data-ttu-id="35df7-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35df7-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```




