---
title: omaSettingDateTime-Ressourcentyp
description: DateTime-Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: afd66ce8838abc3ade8857ec5a4bda74144d6792
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865183"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="8d053-103">omaSettingDateTime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8d053-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="8d053-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d053-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d053-105">DateTime-Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="8d053-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="8d053-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="8d053-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d053-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8d053-107">Properties</span></span>
|<span data-ttu-id="8d053-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d053-108">Property</span></span>|<span data-ttu-id="8d053-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8d053-109">Type</span></span>|<span data-ttu-id="8d053-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d053-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d053-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8d053-111">displayName</span></span>|<span data-ttu-id="8d053-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d053-112">String</span></span>|<span data-ttu-id="8d053-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="8d053-113">Display Name.</span></span> <span data-ttu-id="8d053-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8d053-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8d053-115">description</span><span class="sxs-lookup"><span data-stu-id="8d053-115">description</span></span>|<span data-ttu-id="8d053-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d053-116">String</span></span>|<span data-ttu-id="8d053-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="8d053-117">Description.</span></span> <span data-ttu-id="8d053-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8d053-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8d053-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8d053-119">omaUri</span></span>|<span data-ttu-id="8d053-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d053-120">String</span></span>|<span data-ttu-id="8d053-121">OMA</span><span class="sxs-lookup"><span data-stu-id="8d053-121">OMA.</span></span> <span data-ttu-id="8d053-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8d053-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8d053-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8d053-123">value</span></span>|<span data-ttu-id="8d053-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d053-124">DateTimeOffset</span></span>|<span data-ttu-id="8d053-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="8d053-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d053-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8d053-126">Relationships</span></span>
<span data-ttu-id="8d053-127">Keine</span><span class="sxs-lookup"><span data-stu-id="8d053-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8d053-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8d053-128">JSON Representation</span></span>
<span data-ttu-id="8d053-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8d053-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



