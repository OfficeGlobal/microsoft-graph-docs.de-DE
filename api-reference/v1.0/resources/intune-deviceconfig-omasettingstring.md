---
title: omaSettingString-Ressourcentyp
description: Zeichenfolgendefinition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 890d636afb29fbfb188e9c1b514eecc6360001b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841349"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="1e885-103">omaSettingString-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1e885-103">omaSettingString resource type</span></span>

> <span data-ttu-id="1e885-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1e885-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e885-105">Zeichenfolgendefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="1e885-105">OMA Settings String definition.</span></span>

<span data-ttu-id="1e885-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="1e885-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e885-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1e885-107">Properties</span></span>
|<span data-ttu-id="1e885-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e885-108">Property</span></span>|<span data-ttu-id="1e885-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1e885-109">Type</span></span>|<span data-ttu-id="1e885-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e885-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e885-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1e885-111">displayName</span></span>|<span data-ttu-id="1e885-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e885-112">String</span></span>|<span data-ttu-id="1e885-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="1e885-113">Display Name.</span></span> <span data-ttu-id="1e885-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1e885-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1e885-115">description</span><span class="sxs-lookup"><span data-stu-id="1e885-115">description</span></span>|<span data-ttu-id="1e885-116">String</span><span class="sxs-lookup"><span data-stu-id="1e885-116">String</span></span>|<span data-ttu-id="1e885-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="1e885-117">Description.</span></span> <span data-ttu-id="1e885-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1e885-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1e885-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="1e885-119">omaUri</span></span>|<span data-ttu-id="1e885-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e885-120">String</span></span>|<span data-ttu-id="1e885-121">OMA</span><span class="sxs-lookup"><span data-stu-id="1e885-121">OMA.</span></span> <span data-ttu-id="1e885-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1e885-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1e885-123">Wert</span><span class="sxs-lookup"><span data-stu-id="1e885-123">value</span></span>|<span data-ttu-id="1e885-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e885-124">String</span></span>|<span data-ttu-id="1e885-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="1e885-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e885-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1e885-126">Relationships</span></span>
<span data-ttu-id="1e885-127">Keine</span><span class="sxs-lookup"><span data-stu-id="1e885-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e885-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1e885-128">JSON Representation</span></span>
<span data-ttu-id="1e885-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1e885-129">Here is a JSON representation of the resource.</span></span>
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



