---
title: omaSettingBase64-Ressourcentyp
description: Base64-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f1c6a488adf2f39b2c415e31c4919380ebda5ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982568"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="5d3e9-103">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5d3e9-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="5d3e9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5d3e9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d3e9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5d3e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d3e9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d3e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d3e9-107">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="5d3e9-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="5d3e9-108">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5d3e9-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5d3e9-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5d3e9-109">Properties</span></span>
|<span data-ttu-id="5d3e9-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d3e9-110">Property</span></span>|<span data-ttu-id="5d3e9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5d3e9-111">Type</span></span>|<span data-ttu-id="5d3e9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d3e9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d3e9-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5d3e9-113">displayName</span></span>|<span data-ttu-id="5d3e9-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d3e9-114">String</span></span>|<span data-ttu-id="5d3e9-115">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="5d3e9-115">Display Name.</span></span> <span data-ttu-id="5d3e9-116">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5d3e9-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5d3e9-117">description</span><span class="sxs-lookup"><span data-stu-id="5d3e9-117">description</span></span>|<span data-ttu-id="5d3e9-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d3e9-118">String</span></span>|<span data-ttu-id="5d3e9-119">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="5d3e9-119">Description.</span></span> <span data-ttu-id="5d3e9-120">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5d3e9-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5d3e9-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="5d3e9-121">omaUri</span></span>|<span data-ttu-id="5d3e9-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d3e9-122">String</span></span>|<span data-ttu-id="5d3e9-123">OMA</span><span class="sxs-lookup"><span data-stu-id="5d3e9-123">OMA.</span></span> <span data-ttu-id="5d3e9-124">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5d3e9-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5d3e9-125">fileName</span><span class="sxs-lookup"><span data-stu-id="5d3e9-125">fileName</span></span>|<span data-ttu-id="5d3e9-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d3e9-126">String</span></span>|<span data-ttu-id="5d3e9-127">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="5d3e9-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="5d3e9-128">.CRT</span><span class="sxs-lookup"><span data-stu-id="5d3e9-128">\*.crt</span></span> | <span data-ttu-id="5d3e9-129">p7b</span><span class="sxs-lookup"><span data-stu-id="5d3e9-129">\*.p7b</span></span> | <span data-ttu-id="5d3e9-130">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="5d3e9-130">\*.bin).</span></span>|
|<span data-ttu-id="5d3e9-131">Wert</span><span class="sxs-lookup"><span data-stu-id="5d3e9-131">value</span></span>|<span data-ttu-id="5d3e9-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d3e9-132">String</span></span>|<span data-ttu-id="5d3e9-133">Wert</span><span class="sxs-lookup"><span data-stu-id="5d3e9-133">Value.</span></span> <span data-ttu-id="5d3e9-134">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="5d3e9-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d3e9-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5d3e9-135">Relationships</span></span>
<span data-ttu-id="5d3e9-136">Keine</span><span class="sxs-lookup"><span data-stu-id="5d3e9-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d3e9-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5d3e9-137">JSON Representation</span></span>
<span data-ttu-id="5d3e9-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5d3e9-138">Here is a JSON representation of the resource.</span></span>
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





