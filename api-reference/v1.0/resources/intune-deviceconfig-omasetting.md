---
title: omaSetting-Ressourcentyp
description: Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86cb06b35a0f64052860c268764696a1db8459e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888382"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="ef7c4-103">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ef7c4-103">omaSetting resource type</span></span>

> <span data-ttu-id="ef7c4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ef7c4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef7c4-105">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="ef7c4-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="ef7c4-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ef7c4-106">Properties</span></span>
|<span data-ttu-id="ef7c4-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef7c4-107">Property</span></span>|<span data-ttu-id="ef7c4-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ef7c4-108">Type</span></span>|<span data-ttu-id="ef7c4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef7c4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef7c4-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ef7c4-110">displayName</span></span>|<span data-ttu-id="ef7c4-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef7c4-111">String</span></span>|<span data-ttu-id="ef7c4-112">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="ef7c4-112">Display Name.</span></span>|
|<span data-ttu-id="ef7c4-113">description</span><span class="sxs-lookup"><span data-stu-id="ef7c4-113">description</span></span>|<span data-ttu-id="ef7c4-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef7c4-114">String</span></span>|<span data-ttu-id="ef7c4-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="ef7c4-115">Description.</span></span>|
|<span data-ttu-id="ef7c4-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="ef7c4-116">omaUri</span></span>|<span data-ttu-id="ef7c4-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef7c4-117">String</span></span>|<span data-ttu-id="ef7c4-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="ef7c4-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef7c4-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ef7c4-119">Relationships</span></span>
<span data-ttu-id="ef7c4-120">Keine</span><span class="sxs-lookup"><span data-stu-id="ef7c4-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ef7c4-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ef7c4-121">JSON Representation</span></span>
<span data-ttu-id="ef7c4-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ef7c4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



