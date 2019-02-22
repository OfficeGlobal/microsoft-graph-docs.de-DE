---
title: omaSettingInteger-Ressourcentyp
description: Ganzzahl-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb87ecf7f658e9eb6ed19904a09460d2b2695be4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172324"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="877d4-103">omaSettingInteger-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="877d4-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="877d4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="877d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="877d4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="877d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="877d4-106">Ganzzahl-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="877d4-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="877d4-107">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="877d4-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="877d4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="877d4-108">Properties</span></span>
|<span data-ttu-id="877d4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="877d4-109">Property</span></span>|<span data-ttu-id="877d4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="877d4-110">Type</span></span>|<span data-ttu-id="877d4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="877d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="877d4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="877d4-112">displayName</span></span>|<span data-ttu-id="877d4-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="877d4-113">String</span></span>|<span data-ttu-id="877d4-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="877d4-114">Display Name.</span></span> <span data-ttu-id="877d4-115">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="877d4-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="877d4-116">description</span><span class="sxs-lookup"><span data-stu-id="877d4-116">description</span></span>|<span data-ttu-id="877d4-117">String</span><span class="sxs-lookup"><span data-stu-id="877d4-117">String</span></span>|<span data-ttu-id="877d4-118">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="877d4-118">Description.</span></span> <span data-ttu-id="877d4-119">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="877d4-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="877d4-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="877d4-120">omaUri</span></span>|<span data-ttu-id="877d4-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="877d4-121">String</span></span>|<span data-ttu-id="877d4-122">OMA</span><span class="sxs-lookup"><span data-stu-id="877d4-122">OMA.</span></span> <span data-ttu-id="877d4-123">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="877d4-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="877d4-124">value</span><span class="sxs-lookup"><span data-stu-id="877d4-124">value</span></span>|<span data-ttu-id="877d4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="877d4-125">Int32</span></span>|<span data-ttu-id="877d4-126">Wert</span><span class="sxs-lookup"><span data-stu-id="877d4-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="877d4-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="877d4-127">Relationships</span></span>
<span data-ttu-id="877d4-128">Keine</span><span class="sxs-lookup"><span data-stu-id="877d4-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="877d4-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="877d4-129">JSON Representation</span></span>
<span data-ttu-id="877d4-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="877d4-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```




