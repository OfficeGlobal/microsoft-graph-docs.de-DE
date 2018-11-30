---
title: omaSettingInteger-Ressourcentyp
description: Ganzzahl-Definition der OMA-Einstellungen
ms.openlocfilehash: 36c22b423161d9f3c58c3085fb7b040c663d460b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019509"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="cb4d2-103">omaSettingInteger-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cb4d2-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="cb4d2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cb4d2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb4d2-105">Ganzzahl-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="cb4d2-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="cb4d2-106">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb4d2-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb4d2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb4d2-107">Properties</span></span>
|<span data-ttu-id="cb4d2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb4d2-108">Property</span></span>|<span data-ttu-id="cb4d2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="cb4d2-109">Type</span></span>|<span data-ttu-id="cb4d2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb4d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb4d2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cb4d2-111">displayName</span></span>|<span data-ttu-id="cb4d2-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb4d2-112">String</span></span>|<span data-ttu-id="cb4d2-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="cb4d2-113">Display Name.</span></span> <span data-ttu-id="cb4d2-114">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb4d2-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb4d2-115">description</span><span class="sxs-lookup"><span data-stu-id="cb4d2-115">description</span></span>|<span data-ttu-id="cb4d2-116">String</span><span class="sxs-lookup"><span data-stu-id="cb4d2-116">String</span></span>|<span data-ttu-id="cb4d2-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="cb4d2-117">Description.</span></span> <span data-ttu-id="cb4d2-118">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb4d2-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb4d2-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="cb4d2-119">omaUri</span></span>|<span data-ttu-id="cb4d2-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb4d2-120">String</span></span>|<span data-ttu-id="cb4d2-121">OMA</span><span class="sxs-lookup"><span data-stu-id="cb4d2-121">OMA.</span></span> <span data-ttu-id="cb4d2-122">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cb4d2-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cb4d2-123">value</span><span class="sxs-lookup"><span data-stu-id="cb4d2-123">value</span></span>|<span data-ttu-id="cb4d2-124">Int32</span><span class="sxs-lookup"><span data-stu-id="cb4d2-124">Int32</span></span>|<span data-ttu-id="cb4d2-125">Wert</span><span class="sxs-lookup"><span data-stu-id="cb4d2-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb4d2-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cb4d2-126">Relationships</span></span>
<span data-ttu-id="cb4d2-127">Keine</span><span class="sxs-lookup"><span data-stu-id="cb4d2-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb4d2-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb4d2-128">JSON Representation</span></span>
<span data-ttu-id="cb4d2-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb4d2-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



