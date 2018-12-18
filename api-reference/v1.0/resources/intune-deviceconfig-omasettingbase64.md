---
title: omaSettingBase64-Ressourcentyp
description: Base64-Definition der OMA-Einstellungen
author: tfitzmac
ms.openlocfilehash: 6b0835864d3ec8f8364a15ff293a75dfeded3a0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343722"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="af84b-103">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="af84b-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="af84b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="af84b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af84b-105">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="af84b-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="af84b-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="af84b-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af84b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="af84b-107">Properties</span></span>
|<span data-ttu-id="af84b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af84b-108">Property</span></span>|<span data-ttu-id="af84b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="af84b-109">Type</span></span>|<span data-ttu-id="af84b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af84b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af84b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="af84b-111">displayName</span></span>|<span data-ttu-id="af84b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af84b-112">String</span></span>|<span data-ttu-id="af84b-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="af84b-113">Display Name.</span></span> <span data-ttu-id="af84b-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="af84b-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="af84b-115">description</span><span class="sxs-lookup"><span data-stu-id="af84b-115">description</span></span>|<span data-ttu-id="af84b-116">String</span><span class="sxs-lookup"><span data-stu-id="af84b-116">String</span></span>|<span data-ttu-id="af84b-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="af84b-117">Description.</span></span> <span data-ttu-id="af84b-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="af84b-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="af84b-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="af84b-119">omaUri</span></span>|<span data-ttu-id="af84b-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af84b-120">String</span></span>|<span data-ttu-id="af84b-121">OMA</span><span class="sxs-lookup"><span data-stu-id="af84b-121">OMA.</span></span> <span data-ttu-id="af84b-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="af84b-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="af84b-123">fileName</span><span class="sxs-lookup"><span data-stu-id="af84b-123">fileName</span></span>|<span data-ttu-id="af84b-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af84b-124">String</span></span>|<span data-ttu-id="af84b-125">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="af84b-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="af84b-126">.CRT</span><span class="sxs-lookup"><span data-stu-id="af84b-126">\*.crt</span></span> | <span data-ttu-id="af84b-127">p7b</span><span class="sxs-lookup"><span data-stu-id="af84b-127">\*.p7b</span></span> | <span data-ttu-id="af84b-128">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="af84b-128">\*.bin).</span></span>|
|<span data-ttu-id="af84b-129">Wert</span><span class="sxs-lookup"><span data-stu-id="af84b-129">value</span></span>|<span data-ttu-id="af84b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af84b-130">String</span></span>|<span data-ttu-id="af84b-131">Wert</span><span class="sxs-lookup"><span data-stu-id="af84b-131">Value.</span></span> <span data-ttu-id="af84b-132">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="af84b-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="af84b-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="af84b-133">Relationships</span></span>
<span data-ttu-id="af84b-134">Keine</span><span class="sxs-lookup"><span data-stu-id="af84b-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="af84b-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="af84b-135">JSON Representation</span></span>
<span data-ttu-id="af84b-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="af84b-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



