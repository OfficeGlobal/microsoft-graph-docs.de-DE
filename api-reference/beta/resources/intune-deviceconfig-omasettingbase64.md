---
title: omaSettingBase64-Ressourcentyp
description: Base64-Definition der OMA-Einstellungen
author: tfitzmac
ms.openlocfilehash: ee25db94cc1426194166a7c66b9a8a626d62c3e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304074"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="d04be-103">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d04be-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="d04be-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d04be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d04be-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d04be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d04be-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d04be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d04be-107">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="d04be-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="d04be-108">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d04be-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d04be-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d04be-109">Properties</span></span>
|<span data-ttu-id="d04be-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d04be-110">Property</span></span>|<span data-ttu-id="d04be-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d04be-111">Type</span></span>|<span data-ttu-id="d04be-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d04be-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d04be-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d04be-113">displayName</span></span>|<span data-ttu-id="d04be-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d04be-114">String</span></span>|<span data-ttu-id="d04be-115">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="d04be-115">Display Name.</span></span> <span data-ttu-id="d04be-116">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d04be-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d04be-117">description</span><span class="sxs-lookup"><span data-stu-id="d04be-117">description</span></span>|<span data-ttu-id="d04be-118">String</span><span class="sxs-lookup"><span data-stu-id="d04be-118">String</span></span>|<span data-ttu-id="d04be-119">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="d04be-119">Description.</span></span> <span data-ttu-id="d04be-120">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d04be-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d04be-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="d04be-121">omaUri</span></span>|<span data-ttu-id="d04be-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d04be-122">String</span></span>|<span data-ttu-id="d04be-123">OMA</span><span class="sxs-lookup"><span data-stu-id="d04be-123">OMA.</span></span> <span data-ttu-id="d04be-124">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d04be-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d04be-125">fileName</span><span class="sxs-lookup"><span data-stu-id="d04be-125">fileName</span></span>|<span data-ttu-id="d04be-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d04be-126">String</span></span>|<span data-ttu-id="d04be-127">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="d04be-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="d04be-128">.CRT</span><span class="sxs-lookup"><span data-stu-id="d04be-128">\*.crt</span></span> | <span data-ttu-id="d04be-129">p7b</span><span class="sxs-lookup"><span data-stu-id="d04be-129">\*.p7b</span></span> | <span data-ttu-id="d04be-130">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="d04be-130">\*.bin).</span></span>|
|<span data-ttu-id="d04be-131">Wert</span><span class="sxs-lookup"><span data-stu-id="d04be-131">value</span></span>|<span data-ttu-id="d04be-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d04be-132">String</span></span>|<span data-ttu-id="d04be-133">Wert</span><span class="sxs-lookup"><span data-stu-id="d04be-133">Value.</span></span> <span data-ttu-id="d04be-134">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="d04be-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d04be-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d04be-135">Relationships</span></span>
<span data-ttu-id="d04be-136">Keine</span><span class="sxs-lookup"><span data-stu-id="d04be-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d04be-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d04be-137">JSON Representation</span></span>
<span data-ttu-id="d04be-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d04be-138">Here is a JSON representation of the resource.</span></span>
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





