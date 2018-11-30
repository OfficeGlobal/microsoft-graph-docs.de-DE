---
title: omaSettingBase64-Ressourcentyp
description: Base64-Definition der OMA-Einstellungen
ms.openlocfilehash: 891c13a4cfcc8c0cf378cb5c7f9c6449bd876b7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018628"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="26bad-103">omaSettingBase64-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="26bad-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="26bad-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="26bad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26bad-105">Base64-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="26bad-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="26bad-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="26bad-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="26bad-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="26bad-107">Properties</span></span>
|<span data-ttu-id="26bad-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26bad-108">Property</span></span>|<span data-ttu-id="26bad-109">Typ</span><span class="sxs-lookup"><span data-stu-id="26bad-109">Type</span></span>|<span data-ttu-id="26bad-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26bad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26bad-111">displayName</span><span class="sxs-lookup"><span data-stu-id="26bad-111">displayName</span></span>|<span data-ttu-id="26bad-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26bad-112">String</span></span>|<span data-ttu-id="26bad-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="26bad-113">Display Name.</span></span> <span data-ttu-id="26bad-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="26bad-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="26bad-115">description</span><span class="sxs-lookup"><span data-stu-id="26bad-115">description</span></span>|<span data-ttu-id="26bad-116">String</span><span class="sxs-lookup"><span data-stu-id="26bad-116">String</span></span>|<span data-ttu-id="26bad-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="26bad-117">Description.</span></span> <span data-ttu-id="26bad-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="26bad-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="26bad-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="26bad-119">omaUri</span></span>|<span data-ttu-id="26bad-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26bad-120">String</span></span>|<span data-ttu-id="26bad-121">OMA</span><span class="sxs-lookup"><span data-stu-id="26bad-121">OMA.</span></span> <span data-ttu-id="26bad-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="26bad-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="26bad-123">fileName</span><span class="sxs-lookup"><span data-stu-id="26bad-123">fileName</span></span>|<span data-ttu-id="26bad-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26bad-124">String</span></span>|<span data-ttu-id="26bad-125">Die dem Dateinamen zugeordnete Werteigenschaft (\*.cer</span><span class="sxs-lookup"><span data-stu-id="26bad-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="26bad-126">.CRT</span><span class="sxs-lookup"><span data-stu-id="26bad-126">\*.crt</span></span> | <span data-ttu-id="26bad-127">p7b</span><span class="sxs-lookup"><span data-stu-id="26bad-127">\*.p7b</span></span> | <span data-ttu-id="26bad-128">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="26bad-128">\*.bin).</span></span>|
|<span data-ttu-id="26bad-129">Wert</span><span class="sxs-lookup"><span data-stu-id="26bad-129">value</span></span>|<span data-ttu-id="26bad-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="26bad-130">String</span></span>|<span data-ttu-id="26bad-131">Wert</span><span class="sxs-lookup"><span data-stu-id="26bad-131">Value.</span></span> <span data-ttu-id="26bad-132">(Base64-codierte Zeichenfolge)</span><span class="sxs-lookup"><span data-stu-id="26bad-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="26bad-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="26bad-133">Relationships</span></span>
<span data-ttu-id="26bad-134">Keine</span><span class="sxs-lookup"><span data-stu-id="26bad-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26bad-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="26bad-135">JSON Representation</span></span>
<span data-ttu-id="26bad-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="26bad-136">Here is a JSON representation of the resource.</span></span>
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



