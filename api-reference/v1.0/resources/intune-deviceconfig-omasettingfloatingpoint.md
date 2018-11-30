---
title: omaSettingFloatingPoint-Ressourcentyp
description: Gleitkommadefinition der OMA-Einstellungen.
ms.openlocfilehash: 649e3b3d7716122610ac60291ef58cc25e32c4e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017731"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="95435-103">omaSettingFloatingPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="95435-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="95435-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="95435-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95435-105">Gleitkommadefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="95435-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="95435-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="95435-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95435-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="95435-107">Properties</span></span>
|<span data-ttu-id="95435-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95435-108">Property</span></span>|<span data-ttu-id="95435-109">Typ</span><span class="sxs-lookup"><span data-stu-id="95435-109">Type</span></span>|<span data-ttu-id="95435-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95435-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95435-111">displayName</span><span class="sxs-lookup"><span data-stu-id="95435-111">displayName</span></span>|<span data-ttu-id="95435-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95435-112">String</span></span>|<span data-ttu-id="95435-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="95435-113">Display Name.</span></span> <span data-ttu-id="95435-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95435-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95435-115">description</span><span class="sxs-lookup"><span data-stu-id="95435-115">description</span></span>|<span data-ttu-id="95435-116">String</span><span class="sxs-lookup"><span data-stu-id="95435-116">String</span></span>|<span data-ttu-id="95435-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="95435-117">Description.</span></span> <span data-ttu-id="95435-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95435-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95435-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="95435-119">omaUri</span></span>|<span data-ttu-id="95435-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95435-120">String</span></span>|<span data-ttu-id="95435-121">OMA</span><span class="sxs-lookup"><span data-stu-id="95435-121">OMA.</span></span> <span data-ttu-id="95435-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95435-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95435-123">Wert</span><span class="sxs-lookup"><span data-stu-id="95435-123">value</span></span>|<span data-ttu-id="95435-124">Einzelner</span><span class="sxs-lookup"><span data-stu-id="95435-124">Single</span></span>|<span data-ttu-id="95435-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="95435-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95435-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="95435-126">Relationships</span></span>
<span data-ttu-id="95435-127">Keine</span><span class="sxs-lookup"><span data-stu-id="95435-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="95435-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="95435-128">JSON Representation</span></span>
<span data-ttu-id="95435-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="95435-129">Here is a JSON representation of the resource.</span></span>
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



