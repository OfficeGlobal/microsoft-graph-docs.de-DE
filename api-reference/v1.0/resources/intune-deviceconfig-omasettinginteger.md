---
title: omaSettingInteger-Ressourcentyp
description: Ganzzahl-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f40d5d225c2b4b99573c482b39f886bcd463e9fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860452"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="49d15-103">omaSettingInteger-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="49d15-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="49d15-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="49d15-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49d15-105">Ganzzahl-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="49d15-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="49d15-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="49d15-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49d15-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="49d15-107">Properties</span></span>
|<span data-ttu-id="49d15-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49d15-108">Property</span></span>|<span data-ttu-id="49d15-109">Typ</span><span class="sxs-lookup"><span data-stu-id="49d15-109">Type</span></span>|<span data-ttu-id="49d15-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49d15-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49d15-111">displayName</span><span class="sxs-lookup"><span data-stu-id="49d15-111">displayName</span></span>|<span data-ttu-id="49d15-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49d15-112">String</span></span>|<span data-ttu-id="49d15-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="49d15-113">Display Name.</span></span> <span data-ttu-id="49d15-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="49d15-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="49d15-115">description</span><span class="sxs-lookup"><span data-stu-id="49d15-115">description</span></span>|<span data-ttu-id="49d15-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49d15-116">String</span></span>|<span data-ttu-id="49d15-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="49d15-117">Description.</span></span> <span data-ttu-id="49d15-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="49d15-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="49d15-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="49d15-119">omaUri</span></span>|<span data-ttu-id="49d15-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="49d15-120">String</span></span>|<span data-ttu-id="49d15-121">OMA</span><span class="sxs-lookup"><span data-stu-id="49d15-121">OMA.</span></span> <span data-ttu-id="49d15-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="49d15-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="49d15-123">value</span><span class="sxs-lookup"><span data-stu-id="49d15-123">value</span></span>|<span data-ttu-id="49d15-124">Int32</span><span class="sxs-lookup"><span data-stu-id="49d15-124">Int32</span></span>|<span data-ttu-id="49d15-125">Wert</span><span class="sxs-lookup"><span data-stu-id="49d15-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49d15-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="49d15-126">Relationships</span></span>
<span data-ttu-id="49d15-127">Keine</span><span class="sxs-lookup"><span data-stu-id="49d15-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49d15-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="49d15-128">JSON Representation</span></span>
<span data-ttu-id="49d15-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="49d15-129">Here is a JSON representation of the resource.</span></span>
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



