---
title: omaSettingDateTime-Ressourcentyp
description: DateTime-Definition der OMA-Einstellungen.
author: tfitzmac
ms.openlocfilehash: 9a525d031c9f24cf18495d83e22467e103bca6d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363690"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="15499-103">omaSettingDateTime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="15499-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="15499-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15499-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15499-105">DateTime-Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="15499-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="15499-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="15499-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15499-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="15499-107">Properties</span></span>
|<span data-ttu-id="15499-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15499-108">Property</span></span>|<span data-ttu-id="15499-109">Typ</span><span class="sxs-lookup"><span data-stu-id="15499-109">Type</span></span>|<span data-ttu-id="15499-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15499-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15499-111">displayName</span><span class="sxs-lookup"><span data-stu-id="15499-111">displayName</span></span>|<span data-ttu-id="15499-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15499-112">String</span></span>|<span data-ttu-id="15499-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="15499-113">Display Name.</span></span> <span data-ttu-id="15499-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="15499-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="15499-115">description</span><span class="sxs-lookup"><span data-stu-id="15499-115">description</span></span>|<span data-ttu-id="15499-116">String</span><span class="sxs-lookup"><span data-stu-id="15499-116">String</span></span>|<span data-ttu-id="15499-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="15499-117">Description.</span></span> <span data-ttu-id="15499-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="15499-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="15499-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="15499-119">omaUri</span></span>|<span data-ttu-id="15499-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15499-120">String</span></span>|<span data-ttu-id="15499-121">OMA</span><span class="sxs-lookup"><span data-stu-id="15499-121">OMA.</span></span> <span data-ttu-id="15499-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="15499-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="15499-123">Wert</span><span class="sxs-lookup"><span data-stu-id="15499-123">value</span></span>|<span data-ttu-id="15499-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15499-124">DateTimeOffset</span></span>|<span data-ttu-id="15499-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="15499-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15499-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="15499-126">Relationships</span></span>
<span data-ttu-id="15499-127">Keine</span><span class="sxs-lookup"><span data-stu-id="15499-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15499-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="15499-128">JSON Representation</span></span>
<span data-ttu-id="15499-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="15499-129">Here is a JSON representation of the resource.</span></span>
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



