---
title: omaSettingBoolean-Ressourcentyp
description: Boolesche Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0b3f2d04c9476cc10a67c1e68ba9a29288e8875
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986635"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="223ad-103">omaSettingBoolean-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="223ad-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="223ad-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="223ad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="223ad-105">Boolesche Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="223ad-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="223ad-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="223ad-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="223ad-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="223ad-107">Properties</span></span>
|<span data-ttu-id="223ad-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="223ad-108">Property</span></span>|<span data-ttu-id="223ad-109">Typ</span><span class="sxs-lookup"><span data-stu-id="223ad-109">Type</span></span>|<span data-ttu-id="223ad-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="223ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="223ad-111">displayName</span><span class="sxs-lookup"><span data-stu-id="223ad-111">displayName</span></span>|<span data-ttu-id="223ad-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="223ad-112">String</span></span>|<span data-ttu-id="223ad-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="223ad-113">Display Name.</span></span> <span data-ttu-id="223ad-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="223ad-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="223ad-115">description</span><span class="sxs-lookup"><span data-stu-id="223ad-115">description</span></span>|<span data-ttu-id="223ad-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="223ad-116">String</span></span>|<span data-ttu-id="223ad-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="223ad-117">Description.</span></span> <span data-ttu-id="223ad-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="223ad-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="223ad-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="223ad-119">omaUri</span></span>|<span data-ttu-id="223ad-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="223ad-120">String</span></span>|<span data-ttu-id="223ad-121">OMA</span><span class="sxs-lookup"><span data-stu-id="223ad-121">OMA.</span></span> <span data-ttu-id="223ad-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="223ad-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="223ad-123">Wert</span><span class="sxs-lookup"><span data-stu-id="223ad-123">value</span></span>|<span data-ttu-id="223ad-124">Boolescher</span><span class="sxs-lookup"><span data-stu-id="223ad-124">Boolean</span></span>|<span data-ttu-id="223ad-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="223ad-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="223ad-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="223ad-126">Relationships</span></span>
<span data-ttu-id="223ad-127">Keine</span><span class="sxs-lookup"><span data-stu-id="223ad-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="223ad-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="223ad-128">JSON Representation</span></span>
<span data-ttu-id="223ad-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="223ad-129">Here is a JSON representation of the resource.</span></span>
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



