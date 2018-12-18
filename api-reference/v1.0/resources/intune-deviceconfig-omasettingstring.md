---
title: omaSettingString-Ressourcentyp
description: Zeichenfolgendefinition der OMA-Einstellungen.
author: tfitzmac
ms.openlocfilehash: a62f6dee2bf0f5a9ca96488625a84ceef5f7c785
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311200"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="9f251-103">omaSettingString-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9f251-103">omaSettingString resource type</span></span>

> <span data-ttu-id="9f251-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9f251-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f251-105">Zeichenfolgendefinition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="9f251-105">OMA Settings String definition.</span></span>

<span data-ttu-id="9f251-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="9f251-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9f251-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9f251-107">Properties</span></span>
|<span data-ttu-id="9f251-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f251-108">Property</span></span>|<span data-ttu-id="9f251-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9f251-109">Type</span></span>|<span data-ttu-id="9f251-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f251-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f251-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9f251-111">displayName</span></span>|<span data-ttu-id="9f251-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9f251-112">String</span></span>|<span data-ttu-id="9f251-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="9f251-113">Display Name.</span></span> <span data-ttu-id="9f251-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9f251-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9f251-115">description</span><span class="sxs-lookup"><span data-stu-id="9f251-115">description</span></span>|<span data-ttu-id="9f251-116">String</span><span class="sxs-lookup"><span data-stu-id="9f251-116">String</span></span>|<span data-ttu-id="9f251-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="9f251-117">Description.</span></span> <span data-ttu-id="9f251-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9f251-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9f251-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="9f251-119">omaUri</span></span>|<span data-ttu-id="9f251-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9f251-120">String</span></span>|<span data-ttu-id="9f251-121">OMA</span><span class="sxs-lookup"><span data-stu-id="9f251-121">OMA.</span></span> <span data-ttu-id="9f251-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9f251-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9f251-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9f251-123">value</span></span>|<span data-ttu-id="9f251-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9f251-124">String</span></span>|<span data-ttu-id="9f251-125">Wert.</span><span class="sxs-lookup"><span data-stu-id="9f251-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f251-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9f251-126">Relationships</span></span>
<span data-ttu-id="9f251-127">Keine</span><span class="sxs-lookup"><span data-stu-id="9f251-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f251-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9f251-128">JSON Representation</span></span>
<span data-ttu-id="9f251-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9f251-129">Here is a JSON representation of the resource.</span></span>
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



