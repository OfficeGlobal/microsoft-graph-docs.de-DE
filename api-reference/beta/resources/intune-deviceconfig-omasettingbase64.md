---
title: omaSettingBase64-Ressourcentyp
description: Base64-Definition der OMA-Einstellungen
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f5885a81e68dbea4e5f6f1c8cae456144785338
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413920"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="657e6-103">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="657e6-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="657e6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="657e6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="657e6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="657e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="657e6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="657e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="657e6-107">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="657e6-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="657e6-108">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="657e6-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="657e6-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="657e6-109">Properties</span></span>
|<span data-ttu-id="657e6-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="657e6-110">Property</span></span>|<span data-ttu-id="657e6-111">Typ</span><span class="sxs-lookup"><span data-stu-id="657e6-111">Type</span></span>|<span data-ttu-id="657e6-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="657e6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="657e6-113">displayName</span><span class="sxs-lookup"><span data-stu-id="657e6-113">displayName</span></span>|<span data-ttu-id="657e6-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="657e6-114">String</span></span>|<span data-ttu-id="657e6-115">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="657e6-115">Display Name.</span></span> <span data-ttu-id="657e6-116">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="657e6-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="657e6-117">description</span><span class="sxs-lookup"><span data-stu-id="657e6-117">description</span></span>|<span data-ttu-id="657e6-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="657e6-118">String</span></span>|<span data-ttu-id="657e6-119">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="657e6-119">Description.</span></span> <span data-ttu-id="657e6-120">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="657e6-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="657e6-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="657e6-121">omaUri</span></span>|<span data-ttu-id="657e6-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="657e6-122">String</span></span>|<span data-ttu-id="657e6-123">OMA</span><span class="sxs-lookup"><span data-stu-id="657e6-123">OMA.</span></span> <span data-ttu-id="657e6-124">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="657e6-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="657e6-125">fileName</span><span class="sxs-lookup"><span data-stu-id="657e6-125">fileName</span></span>|<span data-ttu-id="657e6-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="657e6-126">String</span></span>|<span data-ttu-id="657e6-127">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="657e6-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="657e6-128">.CRT</span><span class="sxs-lookup"><span data-stu-id="657e6-128">\*.crt</span></span> | <span data-ttu-id="657e6-129">p7b</span><span class="sxs-lookup"><span data-stu-id="657e6-129">\*.p7b</span></span> | <span data-ttu-id="657e6-130">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="657e6-130">\*.bin).</span></span>|
|<span data-ttu-id="657e6-131">Wert</span><span class="sxs-lookup"><span data-stu-id="657e6-131">value</span></span>|<span data-ttu-id="657e6-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="657e6-132">String</span></span>|<span data-ttu-id="657e6-133">Wert</span><span class="sxs-lookup"><span data-stu-id="657e6-133">Value.</span></span> <span data-ttu-id="657e6-134">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="657e6-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="657e6-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="657e6-135">Relationships</span></span>
<span data-ttu-id="657e6-136">Keine</span><span class="sxs-lookup"><span data-stu-id="657e6-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="657e6-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="657e6-137">JSON Representation</span></span>
<span data-ttu-id="657e6-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="657e6-138">Here is a JSON representation of the resource.</span></span>
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




