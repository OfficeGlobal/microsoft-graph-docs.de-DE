---
title: omaSettingString-Ressourcentyp
description: Zeichenfolgendefinition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0524e077c210f2b13744534b9f42b2bb19d6359b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911763"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="9ff22-103">omaSettingString-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9ff22-103">omaSettingString resource type</span></span>

> <span data-ttu-id="9ff22-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9ff22-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ff22-105">Zeichenfolgendefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="9ff22-105">OMA Settings String definition.</span></span>

<span data-ttu-id="9ff22-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="9ff22-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9ff22-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9ff22-107">Properties</span></span>
|<span data-ttu-id="9ff22-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ff22-108">Property</span></span>|<span data-ttu-id="9ff22-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9ff22-109">Type</span></span>|<span data-ttu-id="9ff22-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ff22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff22-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9ff22-111">displayName</span></span>|<span data-ttu-id="9ff22-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ff22-112">String</span></span>|<span data-ttu-id="9ff22-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="9ff22-113">Display Name.</span></span> <span data-ttu-id="9ff22-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9ff22-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9ff22-115">description</span><span class="sxs-lookup"><span data-stu-id="9ff22-115">description</span></span>|<span data-ttu-id="9ff22-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ff22-116">String</span></span>|<span data-ttu-id="9ff22-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="9ff22-117">Description.</span></span> <span data-ttu-id="9ff22-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9ff22-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9ff22-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="9ff22-119">omaUri</span></span>|<span data-ttu-id="9ff22-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ff22-120">String</span></span>|<span data-ttu-id="9ff22-121">OMA</span><span class="sxs-lookup"><span data-stu-id="9ff22-121">OMA.</span></span> <span data-ttu-id="9ff22-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9ff22-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9ff22-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9ff22-123">value</span></span>|<span data-ttu-id="9ff22-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ff22-124">String</span></span>|<span data-ttu-id="9ff22-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="9ff22-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ff22-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9ff22-126">Relationships</span></span>
<span data-ttu-id="9ff22-127">Keine</span><span class="sxs-lookup"><span data-stu-id="9ff22-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ff22-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9ff22-128">JSON Representation</span></span>
<span data-ttu-id="9ff22-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9ff22-129">Here is a JSON representation of the resource.</span></span>
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



