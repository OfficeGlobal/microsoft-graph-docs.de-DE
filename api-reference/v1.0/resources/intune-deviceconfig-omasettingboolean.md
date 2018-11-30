---
title: omaSettingBoolean-Ressourcentyp
description: Boolesche Definition der OMA-Einstellungen.
ms.openlocfilehash: 1c0cc1d90374b7720fd9ba95e7488a09167f7842
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017399"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="8de6f-103">omaSettingBoolean-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8de6f-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="8de6f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8de6f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8de6f-105">Boolesche Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="8de6f-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="8de6f-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="8de6f-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8de6f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8de6f-107">Properties</span></span>
|<span data-ttu-id="8de6f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8de6f-108">Property</span></span>|<span data-ttu-id="8de6f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8de6f-109">Type</span></span>|<span data-ttu-id="8de6f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8de6f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8de6f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8de6f-111">displayName</span></span>|<span data-ttu-id="8de6f-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8de6f-112">String</span></span>|<span data-ttu-id="8de6f-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="8de6f-113">Display Name.</span></span> <span data-ttu-id="8de6f-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8de6f-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8de6f-115">description</span><span class="sxs-lookup"><span data-stu-id="8de6f-115">description</span></span>|<span data-ttu-id="8de6f-116">String</span><span class="sxs-lookup"><span data-stu-id="8de6f-116">String</span></span>|<span data-ttu-id="8de6f-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="8de6f-117">Description.</span></span> <span data-ttu-id="8de6f-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8de6f-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8de6f-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8de6f-119">omaUri</span></span>|<span data-ttu-id="8de6f-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8de6f-120">String</span></span>|<span data-ttu-id="8de6f-121">OMA</span><span class="sxs-lookup"><span data-stu-id="8de6f-121">OMA.</span></span> <span data-ttu-id="8de6f-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8de6f-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8de6f-123">Wert</span><span class="sxs-lookup"><span data-stu-id="8de6f-123">value</span></span>|<span data-ttu-id="8de6f-124">Boolescher</span><span class="sxs-lookup"><span data-stu-id="8de6f-124">Boolean</span></span>|<span data-ttu-id="8de6f-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="8de6f-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8de6f-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8de6f-126">Relationships</span></span>
<span data-ttu-id="8de6f-127">Keine</span><span class="sxs-lookup"><span data-stu-id="8de6f-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8de6f-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8de6f-128">JSON Representation</span></span>
<span data-ttu-id="8de6f-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8de6f-129">Here is a JSON representation of the resource.</span></span>
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



