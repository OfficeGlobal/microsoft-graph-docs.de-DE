---
title: omaSettingDateTime-Ressourcentyp
description: DateTime-Definition der OMA-Einstellungen.
ms.openlocfilehash: b4ea11c22acb2a4119c2de1934f1ae66c2310658
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016724"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="1e457-103">omaSettingDateTime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1e457-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="1e457-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1e457-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e457-105">DateTime-Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="1e457-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="1e457-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="1e457-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e457-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1e457-107">Properties</span></span>
|<span data-ttu-id="1e457-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e457-108">Property</span></span>|<span data-ttu-id="1e457-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1e457-109">Type</span></span>|<span data-ttu-id="1e457-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e457-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e457-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1e457-111">displayName</span></span>|<span data-ttu-id="1e457-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e457-112">String</span></span>|<span data-ttu-id="1e457-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="1e457-113">Display Name.</span></span> <span data-ttu-id="1e457-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1e457-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1e457-115">description</span><span class="sxs-lookup"><span data-stu-id="1e457-115">description</span></span>|<span data-ttu-id="1e457-116">String</span><span class="sxs-lookup"><span data-stu-id="1e457-116">String</span></span>|<span data-ttu-id="1e457-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="1e457-117">Description.</span></span> <span data-ttu-id="1e457-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1e457-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1e457-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="1e457-119">omaUri</span></span>|<span data-ttu-id="1e457-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e457-120">String</span></span>|<span data-ttu-id="1e457-121">OMA</span><span class="sxs-lookup"><span data-stu-id="1e457-121">OMA.</span></span> <span data-ttu-id="1e457-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1e457-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1e457-123">Wert</span><span class="sxs-lookup"><span data-stu-id="1e457-123">value</span></span>|<span data-ttu-id="1e457-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e457-124">DateTimeOffset</span></span>|<span data-ttu-id="1e457-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="1e457-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e457-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1e457-126">Relationships</span></span>
<span data-ttu-id="1e457-127">Keine</span><span class="sxs-lookup"><span data-stu-id="1e457-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e457-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1e457-128">JSON Representation</span></span>
<span data-ttu-id="1e457-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1e457-129">Here is a JSON representation of the resource.</span></span>
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


