---
title: omaSettingFloatingPoint-Ressourcentyp
description: Gleitkommadefinition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddb11f40faf9db58fefb984fcc08a9fedd66e97d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951551"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="69cfb-103">omaSettingFloatingPoint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="69cfb-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="69cfb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69cfb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69cfb-105">Gleitkommadefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="69cfb-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="69cfb-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="69cfb-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69cfb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69cfb-107">Properties</span></span>
|<span data-ttu-id="69cfb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69cfb-108">Property</span></span>|<span data-ttu-id="69cfb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="69cfb-109">Type</span></span>|<span data-ttu-id="69cfb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69cfb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69cfb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="69cfb-111">displayName</span></span>|<span data-ttu-id="69cfb-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69cfb-112">String</span></span>|<span data-ttu-id="69cfb-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="69cfb-113">Display Name.</span></span> <span data-ttu-id="69cfb-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="69cfb-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="69cfb-115">description</span><span class="sxs-lookup"><span data-stu-id="69cfb-115">description</span></span>|<span data-ttu-id="69cfb-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69cfb-116">String</span></span>|<span data-ttu-id="69cfb-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="69cfb-117">Description.</span></span> <span data-ttu-id="69cfb-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="69cfb-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="69cfb-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="69cfb-119">omaUri</span></span>|<span data-ttu-id="69cfb-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69cfb-120">String</span></span>|<span data-ttu-id="69cfb-121">OMA</span><span class="sxs-lookup"><span data-stu-id="69cfb-121">OMA.</span></span> <span data-ttu-id="69cfb-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="69cfb-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="69cfb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="69cfb-123">value</span></span>|<span data-ttu-id="69cfb-124">Einzelner</span><span class="sxs-lookup"><span data-stu-id="69cfb-124">Single</span></span>|<span data-ttu-id="69cfb-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="69cfb-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69cfb-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69cfb-126">Relationships</span></span>
<span data-ttu-id="69cfb-127">Keine</span><span class="sxs-lookup"><span data-stu-id="69cfb-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="69cfb-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69cfb-128">JSON Representation</span></span>
<span data-ttu-id="69cfb-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="69cfb-129">Here is a JSON representation of the resource.</span></span>
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



