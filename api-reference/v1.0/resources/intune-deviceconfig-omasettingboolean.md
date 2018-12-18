---
title: omaSettingBoolean-Ressourcentyp
description: Boolesche Definition der OMA-Einstellungen.
author: tfitzmac
ms.openlocfilehash: 10101217d1c0f07931cb847e1c14f36844c8dc9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323282"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="a8a34-103">omaSettingBoolean-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a8a34-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="a8a34-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8a34-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8a34-105">Boolesche Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="a8a34-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="a8a34-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="a8a34-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8a34-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8a34-107">Properties</span></span>
|<span data-ttu-id="a8a34-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8a34-108">Property</span></span>|<span data-ttu-id="a8a34-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a8a34-109">Type</span></span>|<span data-ttu-id="a8a34-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8a34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a34-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a8a34-111">displayName</span></span>|<span data-ttu-id="a8a34-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a34-112">String</span></span>|<span data-ttu-id="a8a34-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="a8a34-113">Display Name.</span></span> <span data-ttu-id="a8a34-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8a34-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a8a34-115">description</span><span class="sxs-lookup"><span data-stu-id="a8a34-115">description</span></span>|<span data-ttu-id="a8a34-116">String</span><span class="sxs-lookup"><span data-stu-id="a8a34-116">String</span></span>|<span data-ttu-id="a8a34-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="a8a34-117">Description.</span></span> <span data-ttu-id="a8a34-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8a34-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a8a34-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="a8a34-119">omaUri</span></span>|<span data-ttu-id="a8a34-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8a34-120">String</span></span>|<span data-ttu-id="a8a34-121">OMA</span><span class="sxs-lookup"><span data-stu-id="a8a34-121">OMA.</span></span> <span data-ttu-id="a8a34-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8a34-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a8a34-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a8a34-123">value</span></span>|<span data-ttu-id="a8a34-124">Boolescher</span><span class="sxs-lookup"><span data-stu-id="a8a34-124">Boolean</span></span>|<span data-ttu-id="a8a34-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="a8a34-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8a34-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a8a34-126">Relationships</span></span>
<span data-ttu-id="a8a34-127">Keine</span><span class="sxs-lookup"><span data-stu-id="a8a34-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8a34-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8a34-128">JSON Representation</span></span>
<span data-ttu-id="a8a34-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8a34-129">Here is a JSON representation of the resource.</span></span>
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



