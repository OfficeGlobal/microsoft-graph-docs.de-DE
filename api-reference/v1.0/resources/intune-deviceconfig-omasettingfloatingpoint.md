---
title: omaSettingFloatingPoint-Ressourcentyp
description: Gleitkommadefinition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a36d30cb62862b469d7b32d742275d399ed36db0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888130"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="d3062-103">omaSettingFloatingPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d3062-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="d3062-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d3062-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3062-105">Gleitkommadefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="d3062-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="d3062-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="d3062-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3062-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d3062-107">Properties</span></span>
|<span data-ttu-id="d3062-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3062-108">Property</span></span>|<span data-ttu-id="d3062-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d3062-109">Type</span></span>|<span data-ttu-id="d3062-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3062-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3062-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d3062-111">displayName</span></span>|<span data-ttu-id="d3062-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3062-112">String</span></span>|<span data-ttu-id="d3062-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="d3062-113">Display Name.</span></span> <span data-ttu-id="d3062-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3062-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3062-115">description</span><span class="sxs-lookup"><span data-stu-id="d3062-115">description</span></span>|<span data-ttu-id="d3062-116">String</span><span class="sxs-lookup"><span data-stu-id="d3062-116">String</span></span>|<span data-ttu-id="d3062-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="d3062-117">Description.</span></span> <span data-ttu-id="d3062-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3062-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3062-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d3062-119">omaUri</span></span>|<span data-ttu-id="d3062-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3062-120">String</span></span>|<span data-ttu-id="d3062-121">OMA</span><span class="sxs-lookup"><span data-stu-id="d3062-121">OMA.</span></span> <span data-ttu-id="d3062-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3062-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3062-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d3062-123">value</span></span>|<span data-ttu-id="d3062-124">Einzelner</span><span class="sxs-lookup"><span data-stu-id="d3062-124">Single</span></span>|<span data-ttu-id="d3062-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="d3062-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3062-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d3062-126">Relationships</span></span>
<span data-ttu-id="d3062-127">Keine</span><span class="sxs-lookup"><span data-stu-id="d3062-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3062-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d3062-128">JSON Representation</span></span>
<span data-ttu-id="d3062-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d3062-129">Here is a JSON representation of the resource.</span></span>
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



