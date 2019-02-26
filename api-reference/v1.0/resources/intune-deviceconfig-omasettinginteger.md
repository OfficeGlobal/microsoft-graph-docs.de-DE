---
title: omaSettingInteger-Ressourcentyp
description: Ganzzahl-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e4896af0e43510eb791f37a72a864a405388e9d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253554"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="47a8d-103">omaSettingInteger-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="47a8d-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="47a8d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="47a8d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47a8d-105">Ganzzahl-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="47a8d-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="47a8d-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47a8d-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47a8d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="47a8d-107">Properties</span></span>
|<span data-ttu-id="47a8d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47a8d-108">Property</span></span>|<span data-ttu-id="47a8d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="47a8d-109">Type</span></span>|<span data-ttu-id="47a8d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47a8d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a8d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="47a8d-111">displayName</span></span>|<span data-ttu-id="47a8d-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="47a8d-112">String</span></span>|<span data-ttu-id="47a8d-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="47a8d-113">Display Name.</span></span> <span data-ttu-id="47a8d-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47a8d-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47a8d-115">description</span><span class="sxs-lookup"><span data-stu-id="47a8d-115">description</span></span>|<span data-ttu-id="47a8d-116">String</span><span class="sxs-lookup"><span data-stu-id="47a8d-116">String</span></span>|<span data-ttu-id="47a8d-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="47a8d-117">Description.</span></span> <span data-ttu-id="47a8d-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47a8d-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47a8d-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="47a8d-119">omaUri</span></span>|<span data-ttu-id="47a8d-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="47a8d-120">String</span></span>|<span data-ttu-id="47a8d-121">OMA</span><span class="sxs-lookup"><span data-stu-id="47a8d-121">OMA.</span></span> <span data-ttu-id="47a8d-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47a8d-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47a8d-123">value</span><span class="sxs-lookup"><span data-stu-id="47a8d-123">value</span></span>|<span data-ttu-id="47a8d-124">Int32</span><span class="sxs-lookup"><span data-stu-id="47a8d-124">Int32</span></span>|<span data-ttu-id="47a8d-125">Wert</span><span class="sxs-lookup"><span data-stu-id="47a8d-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47a8d-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="47a8d-126">Relationships</span></span>
<span data-ttu-id="47a8d-127">Keine</span><span class="sxs-lookup"><span data-stu-id="47a8d-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47a8d-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="47a8d-128">JSON Representation</span></span>
<span data-ttu-id="47a8d-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="47a8d-129">Here is a JSON representation of the resource.</span></span>
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



